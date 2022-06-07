# Transferring Issues

Some issues may need to be transferred to another repository after some time. This is especially the case when a discussion started in a private repository to address an internal matters, but after some time (and anonymization if necessary) doesn't contain any [confidential or restricted](../../information-classification.md) anymore, and should therefore be shared publicly in respect of the blindnet Openness Framework.

This can be done [manually](https://docs.github.com/en/issues/tracking-your-work-with-issues/transferring-an-issue-to-another-repository) directly on GitHub, one issue at a time, or in bulck using the GitHub CLI.

## Process

"OF Triage:..." labels should be used to ease the process of identifying issues to be transferred from a private repository to a public one according to the Openness Framework.

### Open Information

Mark all issues to transfer with using the "***OF Triage: open***" label. Then, add the following comment:

> This issue is scheduled to transfer to the {repo-name} public repository on {YYYY-MM-DD at HH pm/ am TimeZone} {optional short explanation of context}.

### Restricted Information

Issues containing restricted information with the "***OF Triage: restricted***".

### To Be Open Information

When some issues are identified to be transferred, but only after a specific requirement has been met (e.g. waiting for some restricted piece of information to go public, or going through an anonymization process), use the "***OF Triage: To Be Open***" label.

### Consent Requirement

If you think the issue contain pieces of information a stakeholder could consider private, use the "***OF Triage: require consent***" and add the following comment:

> {stakeholders' tags}: please consent (:+1:, no comment) or discontent (:-1: + comment) to the transfer of this issue as it is to {repo-name} {optional short explanation of context}

## Transferring Issues in Bulk

The following step-by-step is given for bash on Linux, and require installing the [GitHub CLI](https://cli.github.com/) and [`jq`](https://stedolan.github.io/jq/):

```bash
# login to GitHub
gh auth login

# go to the origin private repository
cd communication-management

# transfer issues with an "OF Triage: open" label, to a private buffer repository
# this is required as issues can't be transfered from a private to a public
# repository directly
gh issue list --label "OF Triage: open" -s all --json number | \
  jq -r '.[] | .number' | \
  xargs -I% gh issue transfer % https://github.com/blindnet-io/___issue-transfer-buffer

# go to the buffer repository
cd ../___issue-transfer-buffer

# make the buffer repository public
gh repo edit --visibility public

# transfer issues to the public repository
gh issue list --label "OF Triage: open" -s all --json number | \
  jq -r '.[] | .number' | \
  xargs -I% gh issue transfer % https://github.com/blindnet-io/devrel-management

# make the buffer repository private again
gh repo edit --visibility private

# go to the destination public repository
cd ../devrel-management

# Remove the "OF Triage: open" label on all transfered issues
gh issue list --label "OF Triage: open" -s all --json number | \
  jq -r '.[] | .number' | \
  xargs -I% gh issue edit % --remove-label "OF Triage: open"   
```

> A big thanks to [James Loh](https://github.com/jloh) for [this idea](https://jloh.co/posts/bulk-migrate-issues-github-cli/).
