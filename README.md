# Purpose
This repo build for testing github action config

# Test config
| workflow | from | function |
| --- | --- | --- |
|[stackoverflow-70666214-1.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/stackoverflow-70666214-1.yml)| https://stackoverflow.com/questions/70666214/github-actions-workflow-run-three-levels-of-workflows | workflow_run event trigger run[^1][^2]  |
|[stackoverflow-70666214-2.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/stackoverflow-70666214-2.yml)| ~ | ~ |
|[stackoverflow-70666214-3.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/stackoverflow-70666214-1.yml)| ~ | ~ |
|[reusable-workflow-caller.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/reusable-workflow-caller.yml)| https://docs.github.com/en/actions/learn-github-actions/reusing-workflows | reusing workflow[^3] |
|[reusable-workflow-A.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/reusable-workflow-A.yml)| ~ | output |
|[reusable-workflow-B.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/reusable-workflow-B.yml)| ~ | input |
|[reusable-workflow-C.yml](https://github.com/bxb100/action-test/blob/main/.github/workflows/reusable-workflow-C.yml)| ~ | deploy[^4] |








[^1]: https://docs.github.com/en/actions/learn-github-actions/events-that-trigger-workflows#workflow_run
[^2]: https://docs.github.com/en/actions/learn-github-actions/workflow-syntax-for-github-actions#on
[^3]: https://docs.github.com/en/actions/learn-github-actions/workflow-syntax-for-github-actions#jobsjob_iduses
[^4]: https://github.com/bxb100/action-test/blob/main/workflow-panel-show.md that's same with doc show
