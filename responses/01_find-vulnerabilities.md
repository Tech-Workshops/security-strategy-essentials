## Finding vulnerable dependencies

Security vulnerabilities can cause a range of problems for your project or the people who use it.  A vulnerability could affect the confidentiality, integrity, or availability of a project.  Sometimes vulnerabilities aren't in the code you write, but in the code your project depends on. Staying up-to-date with the most recent versions is the best line of defense.

This repository has some existing dependencies which will need updating to stay secure.

### How can we identify dependencies and if they are vulnerable?

This repository is a Node.js project utilizing NPM. Because of that, the `package.json` defines this repository's dependencies.  For our time together, we'll be focusing on these JavaScript dependencies. Keep in mind that different programming languages may have different dependency files. You might work with a `Gemfile`, `Gemfile.lock`, `*.gemspec`, `requirements.txt`, `pipfile.lock`, or other files.

How can we know these dependencies are secure? It's not always easy, but GitHub is watching out.

### GitHub's security alerts for vulnerable dependencies

You may notice some alerts from GitHub about this repository. You may get an email, or see a yellow bar warning you about the `package.json` file.

![dependency vulnerability alert](https://user-images.githubusercontent.com/9906718/46882979-c275b680-ce50-11e8-9f47-2081daf20b98.png)

GitHub tracks public vulnerabilities in Ruby gems, NPM, Python, Java, and .Net packages.

GitHub receives a notification of a newly-announced vulnerability. Next, we check for repositories that use the affected version of that dependency. We send security alerts to a set of people within those affected repositories. The owners are contacted by default. But, it's possible to configure specific teams or individuals to get these important notifications.

**GitHub never publicly discloses identified vulnerabilities for any repository.**

## Step 2: Find this repository's vulnerable dependencies

Use GitHub's security alerts to identify a vulnerable NPM dependency.

### :keyboard: Activity: Identify the suggested version update

1. Click the **Insights** tab in your repository.
2. On the left hand navigation bar, click **Dependency graph**.
3. Scroll down until you see a yellow bar highlighting the dependency named `debug`, and click on the right hand side of the yellow `debug` section.
4. Take note of the suggested version.
5. Comment in this issue with the suggested update version.


> _**GitHub Enterprise Server only:** This is all possible on GitHub Enterprise through GitHub Connect. It may take up to an hour to refresh the alerts and make them visible. After waiting a reasonable amount of time, if you are still not seeing the yellow bar in the Dependency Graph, you may want to contact your administrator. In the mean time, to move along with the course, we'll give you a hint - the recommended upgraded version is `2.6.9`._

For a printable version of the steps in this course, check out the [Quick Reference Guide]({{ host }}/public/{{ course.slug }}.pdf).

<hr>
<h3 align="center">Return to this issue for my next comment.</h3>
