Run Drone server & runner in containers:

- dc-start.sh for docker-compose variant
- ans-start.sh for ansible-playbook variant

both use .env file with credentials and host ip, but ansible variant
use encrypted way with Vault (put your pass in vault.pass file).

After start add secrets for Nexus registry in Drone server repo settings,
it will be used in drone.yml file.

Dir repo_for_drone_ci - just test project for pipeline.
