# Config VS-CODE

1. Download profile.
2. Install lint:

### GO
- [golangci-lint](https://golangci-lint.run/)
```
$ brew install golangci-lint 
$ golangci-lint --version 
```

For running golangci-lint we recommend you run it with the following flags:

```
golangci-lint run --max-issues-per-linter=0 --max-same-issues=0 --config=.code_quality/.golangci.yml
```

The flags --max-issues-per-linter=0 and --max-same-issues=0 disable golangci-lint default limit on maximum issues per linter and maximum number of same issues per file. We recommend you keep these flags so you can see all issues detected by the tool and not some of them.

golangci-lint natively provides a way of running and automatically fixing some errors it finds. We purposely don't offer this feature in our pre-commit file. This is because after testing this feature we found it to be unreliable and with the potential of breaking your code. If you still want to use it beware that you may face issues like this one.

### JAVA
- [Google Java Format](https://github.com/google/google-java-format)

google-java-format is a program that reformats Java source code to comply with Google Java Style.
For installing it, you can use Homebrew:


```
$ brew install google-java-format
$ google-java-format --version 
google-java-format: Version 1.11.0
```
- [Checkstyle](https://checkstyle.sourceforge.io/)

The formatter can act on whole files, on limited lines (--lines), on specific offsets (--offset), passing through to standard-out (default) or altered in-place (--replace).

Checkstyle
Checkstyle is a development tool to help programmers write Java code that adheres to a coding standard. It automates the process of checking Java code to spare humans of this boring (but important) task. This makes it ideal for projects that want to enforce a coding standard.
Checkstyle is highly configurable and can be made to support almost any coding standard.
For installing Checkstyle you can use Homebrew:

```
$ brew install checkstyle 
$ checkstyle --version 
Checkstyle version: 8.44
```

- [PMD](https://pmd.github.io/)

PMD is a source code analyzer. It finds common programming flaws like unused variables, empty catch blocks, unnecessary object creation, and so forth.
For installing PMD you can use Homebrew:

```
$ brew install pmd 
$ pmd -h // Help message
```

- [Spotbugs](https://spotbugs.github.io/)

SpotBugs is a program which uses static analysis to look for bugs in Java code. SpotBugs requires JRE (or JDK) 1.8.0 or later to run.
For installing Spotbugs you can use Homebrew:

```
$ brew install spotbugs 
$ spotbugs -textui -version 
// Spotbougs outputs nothing but the exit code ($?) will be 0.
```

- install extencion if not exist and config with file local or file on internet.

![extencion java](/images/java1.png)

![extencion java](/images/java2.png)