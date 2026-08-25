# Contributing to Eclipse daanse

Eclipse daanse is an open source project hosted by the Eclipse Foundation. Contributions are accepted from across the community.

## Issues

If you're having a problem with Eclipse daanse then our first recommendation would be to look at [the documentation](https://www.saanse.org).

If you're still having problems then search the [issue tracker](https://github.com/eclipse-daanse) of the corisponding repo for a relevant issue or create a new one.

## Contributing code

We are always happy to welcome new contributors ❤️. If you want to contribute fixes or enhancements to Eclipse daanse then you can do so using a *triangular workflow*.

* To make things easier for everyone, please start by checking if you have already signed the [ECA](#contributor-license)
* Fork the repository in GitHub and make changes in your fork.
  - Make sure that your changes are small and easy to understand. Separate changes into multiple commits where that makes sense
  - Commit messages should be detailed and descriptive
  - Include automated tests for any bug fixes and new code. Contributions submitted without tests may not be accepted.
  - Each commit should try to do one thing, and the code should build cleanly with each commit
* Submit a pull request to the Eclipse sensiNact repository
  - Relate the pull request to an existing issue or discussion. This will give reviewers context for your changes and make the review process faster 🚀.
  - Make sure that the pull request passes all of the CI checks


### Contributor License

If this is your first time contributing to an Eclipse Foundation project, you'll need to sign the [Eclipse Contributor Agreement][ECA].

- [Create an account](https://dev.eclipse.org/site_login/createaccount.php) on dev.eclipse.org
- Open your [Account Settings tab](https://dev.eclipse.org/site_login/myaccount.php#open_tab_accountsettings), enter your GitHub ID and click Update Account
- Read and [sign the ECA](https://dev.eclipse.org/site_login/myaccount.php#open_tab_cla)
- The email address in your git commits must be the exact same email address you used for your Eclipse account and signing the ECA.


## Contact us

[Join the mailing list](https://accounts.eclipse.org/mailing-list/sensinact-dev) and email the community at sensinact-dev@eclipse.org to discuss your ideas and get help

## Build

The Eclipse sensiNact build requires below as dependencies.

- Java 21+
- Maven 3.9.6+

The Eclipse daanse build uses code generation in some components. Please Run the full build once before attempting to load the code into your IDE.

```bash
mvn install -DskipTests=true
```

Now you can open the project in your IDE and it won't complain about missing files. You'll be able to use the IDE to perform incremental builds and run tests. You should rarely need to run the maven build, except when:

- you want to force a clean build
- your changes affect code generation
- you want to see if your changes will pass the same builds that GitHub Actions runs


## Semantic Versioning

Eclipse daanse version numbers follow [Semantic Versioning](https://semver.org). This means we increment the major version when we make incompatible API changes. This includes any changes which

- break binary compatibility
- break source compatibility


## Coding Style

Eclipse daanse follows a space-indented coding style. There is an Editor Config configuration in the root of the repository that you can use to set up your editor application. The CI checks include Editor Config validation, so please be sure to fix any errors.

For details of how to validate locally please see [the super-linter documentation](https://github.com/super-linter/super-linter/blob/main/docs/run-linter-locally.md).

