# Contributing speaker materials

Thank you for sharing your NIC 2026 session resources!

## Folder structure

Keep all materials for a session in a subfolder under the speaker's name:

```text
Speaker Name/
    Session Title/
        README.md
        slides.pdf
        demos/
```

- Match the speaker and session names in the conference program.
- For a joint session, use one shared speaker folder, for example `Speaker One - Speaker Two`.
- Use folder names that work on Windows, macOS, and Linux. Replace characters such as `:`, `/`, `\`, `?`, `*`, `"`, `<`, `>`, and `|` with a hyphen, and avoid trailing spaces or periods.
- Put only your own session materials in your contribution. Do not change another speaker's files without coordinating with them.
- Copy [templates/session/README.md](templates/session/README.md) into your session folder, replace the placeholders, and remove unused sections.

## Option 1: Upload through GitHub

No local Git installation is required.

1. Click **Fork** on this repository to create your own copy.
2. In your fork, select **Add file > Create new file**. Enter `Speaker Name/Session Title/README.md` as the filename to create the folders and session README.
3. Fill in the README using the template and commit it to your fork.
4. Open the new session folder and select **Add file > Upload files** to add your slides and demos.
5. Select **Contribute > Open pull request**. Confirm that the base repository is `nordicinfrastructureconference/2026` and the base branch is `main`.
6. Describe the materials you added and complete the pull-request checklist.

GitHub's browser upload limit is **25 MiB per file**. Use Git for larger files, or publish a download link instead.

## Option 2: Use Git

Fork the repository first, then clone your fork. For example, in PowerShell:

```powershell
git clone https://github.com/YOUR-USERNAME/2026.git nic-2026
Set-Location nic-2026
git switch -c add-speaker-materials

# Add your speaker/session folders and materials, then:
git add -- "Speaker Name"
git commit -m "Add Speaker Name session materials"
git push -u origin add-speaker-materials
```

Open a pull request from that branch to `nordicinfrastructureconference/2026:main`.

GitHub warns about files larger than **50 MiB** and blocks files larger than **100 MiB** in regular Git. Keep files below 100 MiB. For larger slide decks, recordings, or demo archives, host them elsewhere and include stable download links in the session README.

## Option 3: Send materials to the program manager

Email your materials or download links to [program@nicconf.com](mailto:program@nicconf.com). Include your speaker name, session title, prerequisites, and any related links. Confirm that the submitted materials may be published under this repository's MIT license.

## What to include

- Slides, preferably PDF, with the original slide file if you wish.
- Demo source code or a ZIP archive. Source files are easier for attendees to browse and reuse.
- A README with a short session summary, a list of materials, and setup/run instructions.
- Links to relevant documentation, repositories, and recordings if available.
- Required tools, versions, permissions, estimated cloud costs, and cleanup instructions for demos that provision resources.

## Before submitting

- Remove passwords, API keys, tokens, connection strings, tenant/customer data, and other confidential information. Use clearly marked placeholders and synthetic sample data.
- Check slide notes, screenshots, archives, and Git history as well as source files. Deleting a secret in a later commit does not remove it from history; revoke exposed credentials before submitting.
- Do not include build output, dependency caches, or operating-system/editor metadata.
- Review demo commands for destructive operations. Document prerequisites, costs, and cleanup clearly.
- Check that README links work and that all referenced files are included.
- Confirm that you have the right to publish all contributed material under the [MIT license](LICENSE). Keep required third-party copyright and license notices, and link to content that cannot be redistributed.

Maintainers review pull requests before merging. You can submit updates later using the same process.
