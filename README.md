# builddoctor-flaky-demo

A small, repeatable example of a run that fails on its first attempt and passes when the same commit is run again.

The step "Run tests" in `.github/workflows/ci.yml` fails whenever `github.run_attempt` is 1 and passes on every rerun. It exists to check how [BuildDoctor](https://builddoctor.app) reports a run that passed on retry, before and after the rerun.

There is no real code to test here.
