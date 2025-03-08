333# Purpose
This repo build for testing github action config

# Test config
| workflow | from | function |
| --- | --- | --- |
|[stackoverflow-70666214-1.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/stackoverflow-70666214-1.yml)| <https://stackoverflow.com/questions/70666214/github-actions-workflow-run-three-levels-of-workflows> | workflow_run event trigger run[^1][^2]  |
|[stackoverflow-70666214-2.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/stackoverflow-70666214-2.yml)| ~ | ~ |
|[stackoverflow-70666214-3.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/stackoverflow-70666214-1.yml)| ~ | ~ |
|[reusable-workflow-caller.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/reusable-workflow-caller.yml)| <https://docs.github.com/en/actions/learn-github-actions/reusing-workflows> | reusing workflow[^3][^6] |
|[reusable-workflow-A.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/reusable-workflow-A.yml)| ~ | output |
|[reusable-workflow-B.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/reusable-workflow-B.yml)| ~ | input |
|[reusable-workflow-C.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/reusable-workflow-C.yml)| ~ | deploy[^4] |
|[stackoverflow-68759990.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/stackoverflow-68759990.yml)| <https://stackoverflow.com/questions/68759990/pull-request-is-not-detecting-action-when-run-via-workflow-run> | PR check using reusing way[^5]|
|[stackoverflow-68759990-1.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/stackoverflow-68759990-1.yml)| ~ | ~ |
|[stackoverflow-68759990-2.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/stackoverflow-68759990-2.yml)| ~ | workflow_run test |
|[emoji-notify.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/emoji-notify.yml)| ~ | test notify emoji style|
|[webdav-test-issue-30.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/webdav-test-issue-30.yml)| <https://github.com/bxb100/action-upload-webdav/issues/30> | test github action blob path |
|[adding-a-job-summary.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/adding-a-job-summary.yml)|<https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#adding-a-job-summary>| add job summary[^7] |
|[Dynamic use action*](https://github.com/bxb100/action-test/blob/main/.github/workflows/dynamic-use-action.yml) | <https://github.com/orgs/community/discussions/45342> <br/> [incubator-opendal action](https://github.com/apache/incubator-opendal/blob/331b4a90ba71ff1aa5dc73e63aaeb6e8a4cc92ea/.github/actions/behavior_test_core/action.yaml#L34) | dynamic use action |

> `*` : `${{ toJson(toJson()) }}` same as `'${{ toJson() }}'`

[^1]: <https://docs.github.com/en/actions/learn-github-actions/events-that-trigger-workflows#workflow_run>
[^2]: <https://docs.github.com/en/actions/learn-github-actions/workflow-syntax-for-github-actions#on>
[^3]: <https://docs.github.com/en/actions/learn-github-actions/workflow-syntax-for-github-actions#jobsjob_iduses>
[^4]: <https://github.com/bxb100/action-test/blob/main/workflow-panel-show.md> that's same with doc show
[^5]: <https://github.com/bxb100/action-test/pull/4>
[^6]: <https://github.community/t/ref-head-in-reusable-workflows/203690/30> workflow local reference not working now(20220120)
[^7]: <https://github.com/gradle/gradle-build-action>
