# Normandale DNS

This repository tracks DNS configuration for Normandale Ltd and deploys using [octoDNS](https://octodns.readthedocs.io/en/latest/index.html).

## Hosting

Normandale Domains are hosted on [Mythic Beasts](https://www.mythic-beasts.com/). A UK based hosting provider.

> [!CAUTION]
> Making DNS changes in the Mythic Beasts portal will be overridden/deleted by workflows in this repo.

## Making Changes

1. Fork this repository using the 'Fork' button in the top right of the Github UI.
2. Clone your forked copy:
   ```bash
    git clone https://github.com/<your-username>/<forked-repo-name>
   ```

3. Make your changes, and commit them to your fork.
4. Open a pull request on the upstream repository (https://github.com/normandaleltd/dns)
5. Ensure make sure all the CI/CD checks pass.
   >[!NOTE]
   > You may need to wait for a repository admin to approve the CI/CD workflow runs.

   >[!TIP]
   > You can run the linting checks locally using UV.
   >```bash
   >  uvx pre-commit run --all-files
   >```

6. Your change will be reviewed by an admin and the change will be pushed by a workflow once the Pull Request has been merged.