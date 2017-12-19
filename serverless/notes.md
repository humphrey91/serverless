Service Information
service: notes-app-api
stage: prod
region: us-west-2
stack: notes-app-api-prod
api keys:
  None
endpoints:
  POST - https://8grn2dujc4.execute-api.us-west-2.amazonaws.com/prod/notes
  GET - https://8grn2dujc4.execute-api.us-west-2.amazonaws.com/prod/notes/{id}
  GET - https://8grn2dujc4.execute-api.us-west-2.amazonaws.com/prod/notes
  PUT - https://8grn2dujc4.execute-api.us-west-2.amazonaws.com/prod/notes/{id}
  DELETE - https://8grn2dujc4.execute-api.us-west-2.amazonaws.com/prod/notes/{id}
functions:
  create: notes-app-api-prod-create
  get: notes-app-api-prod-get
  list: notes-app-api-prod-list
  update: notes-app-api-prod-update
  delete: notes-app-api-prod-delete


  us-west-2:616a099f-f69d-4995-976d-edb0d8743ec8


  apig-test \
  --username='humphrey.js@gmail.com' \
  --password='Passw0rd!' \
  --user-pool-id='us-west-2_hzCEnaQzJ' \
  --app-client-id='70d9eotkkgnimb5kljnni9jgtt' \
  --cognito-region='us-west-2' \
  --identity-pool-id='us-west-2:616a099f-f69d-4995-976d-edb0d8743ec8' \
  --invoke-url='https://8grn2dujc4.execute-api.us-west-2.amazonaws.com/prod/notes' \
  --api-gateway-region='us-west-2' \
  --path-template='' \
  --method='POST' \
  --body='{"content":"hello world","attachment":"hello.jpg"}'

fix
