https://docs.github.com/en/rest/migrations/users?apiVersion=2026-03-10#get-a-user-migration-status
https://docs.github.com/en

curl https://google.com
curl https://api.github.com/repos/sunny7899/FastAPI-CRUD/downloads url not found

<YOUR_TOKEN> -  repo, user - roles

If your username is xyz and repo is abc, below will be the command
curl -L -X POST -H "Accept: application/vnd.github+json" -H
"Authorization: Bearer <YOUR_TOKEN>" -H "X-GitHub-Api-Version:
2022-11-28" -d '{"lock_repositories":false,
"repositories":["usernameOrorg/reponame"]}'
https://api.github.com/user/migrations
get node id- >migration id

curl -L -H "Accept: application/vnd.github+json" -H
"Authorization: Bearer <YOUR_TOKEN>" -H "X-GitHub-Api-Version:
2022-11-28" https://api.github.com/user/migrations/MIGRATION_ID
Check the `"state"` field in the JSON response. * If it says `"pending"` or `"exporting"`, wait a few
moments and run the above command again. * When it says `"exported"`, your archive is ready.

curl -L -H "Accept: application/vnd.github+json" -H
"Authorization: Bearer <YOUR_TOKEN>" -H "X-GitHub-Api-Version:
2022-11-28"
https://api.github.com/user/migrations/MIGRATION_ID/archive -o
<your_archive_name>.tar.gz

to check access
curl -L \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  https://api.github.com/repos/<YOUR_ORG_NAME>/ssr

for user migration repos-
curl -L -X POST -H "Accept: application/vnd.github+json" -H
"Authorization: Bearer <YOUR_TOKEN>" -H "X-GitHub-Api-Version:
2022-11-28" -d '{"lock_repositories":false,
"repositories":["<YOUR_REPO>"]}'
https://api.github.com/user/migrations

formatted curl for user migration repos-
curl -L \
  -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/user/migrations \
  -d '{
    "lock_repositories": false,
    "repositories": ["<YOUR_REPO>"]
  }'

check migration state-
curl -L -H "Accept: application/vnd.github+json" -H
"Authorization: Bearer <YOUR_TOKEN>" -H "X-GitHub-Api-Version:
2022-11-28" https://api.github.com/user/migrations/<YOUR_MIGRATION_ID NUMBER>

FORMATTED check migration state-
curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/user/migrations/<YOUR_MIGRATION_ID NUMBER>
  

note error- fix it by updating correct migration id
    "message": "Not Found",
  "documentation_url": "https://docs.github.com/rest/migrations/users#get-a-user-migration-status",
  "status": "404"

List user migrations-
curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2026-03-10" \
  https://api.github.com/user/migrations
  
download archive
curl -L -H "Accept: application/vnd.github+json" -H
"Authorization: Bearer <YOUR_TOKEN>" -H "X-GitHub-Api-Version:
2026-03-10"
https://api.github.com/user/migrations/id/archive -o
sunny-blog-app.tar.gz

curl -o archive.zip "YOUR_POSTMAN_URL"

click on send and download button in postman.save file in .tar.gz format

for orgs repo-
curl -L -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/orgs/<YOUR_ORG_NAME>/migrations \
  --data-raw "{\"lock_repositories\":false,\"repositories\":[\"<YOUR_REPO>\"]}"

  curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/orgs/<YOUR_ORG_NAME>/migrations

  curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/orgs/<YOUR_ORG_NAME>/migrations/<YOUR_MIGRATION_ID_NUMBER>/archive \
  -o ssr-migration.tar.gz


  curl -L -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/orgs/NodeJSEngineering/migrations \
  --data-raw "{\"lock_repositories\":false,\"repositories\":[\"NodeJSEngineering/Node-Task-Queue-system/\"]}"

  curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/orgs/angulardevelopment/migrations


  curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/orgs/NodeJSEngineering/migrations/id/archive \
  -o Node-Task-Queue-system-app.tar.gz

curl -L -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/user/migrations \
  --data-raw "{\"lock_repositories\":false,\"repositories\":[\"sunny7899/blog.sunny.dev\"]}"


https://api.github.com/users/sunny7899/repos
https://api.github.com/orgs/angulardevelopment/repos?per_page=100&page=1
"https://api.github.com/user/repos?per_page=100&page=1"