bot: webhook
---

## Create a post for each repository

- name: repo_name
- message: **Updates for https://github.com/plantuml/repo_name**

___ 

## **Howto create for new repository**

- create a new post :
**title**: `plantuml/plantuml`
**message**: `**Updates for https://github.com/plantuml/plantuml/**`

- copy the post id _(we will use it later)_

- go to the Webhooks configuration in the github repository :
https://github.com/plantuml/plantuml/hooks

- Add a webhook:
**Payload URL**:  `WEBHOOK_URL/github?thread_id=POST_ID`
> replace WEBHOOK_URL and POST_ID with the ones you saved before
**Content type**: `application-json`
**Witch events**:  `every things`
**Active**: `yes`

informations from https://gist.github.com/NikanWasTaken/c5154738fcb04456a199177933d6edbf