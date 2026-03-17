# CI/CD Workflow Test - N8N

This file was created to test the GitHub Actions CI/CD workflow for N8N.

## Test Information

- **Date**: 2026-03-16
- **Purpose**: Verify automated deployment workflow for official Docker image
- **Expected Behavior**: 
  - GitHub Actions triggers on push to main
  - SSH connection to VPS (46.202.195.222)
  - Docker compose pull (NOT git pull - official image)
  - Docker compose up -d with new image
  - Health check for n8n-production container
  - NO rollback (official image deployment)

## Test Status

- [ ] Workflow triggered
- [ ] Image pull completed
- [ ] Container restart completed
- [ ] Health check passed
- [ ] Service running correctly

## Notes

This is a test commit to verify the CI/CD pipeline is working correctly.
N8N uses official Docker image - no git pull, only docker compose pull.
Container: n8n-production (port 5678)
