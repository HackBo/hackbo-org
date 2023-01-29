<<<<<<< HEAD
# Main



## Getting started

To make it easy for you to get started with GitLab, here's a list of recommended next steps.

Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!

## Add your files

- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:

```
cd existing_repo
git remote add origin https://gitlab.com/hackbo/main.git
git branch -M main
git push -uf origin main
```

## Integrate with your tools

- [ ] [Set up project integrations](https://gitlab.com/hackbo/main/-/settings/integrations)

## Collaborate with your team

- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)

## Test and Deploy

Use the built-in continuous integration in GitLab.

- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)

***

# Editing this README

When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.

## Suggestions for a good README
Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.

## Name
Choose a self-explaining name for your project.

## Description
Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.

## Badges
On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.

## Visuals
Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.

## Installation
Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.

## Usage
Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.

## Support
Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.

## Roadmap
If you have ideas for releases in the future, it is a good idea to list them in the README.

## Contributing
State if you are open to contributions and what your requirements are for accepting them.

For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.

You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.

## Authors and acknowledgment
Show your appreciation to those who have contributed to the project.

## License
For open source projects, say how it is licensed.

## Project status
If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
=======
Example [Hugo](https://gohugo.io) website using [GitLab Pages](https://about.gitlab.com/stages-devops-lifecycle/pages/).

Learn more about GitLab Pages at the [official documentation](https://docs.gitlab.com/ce/user/project/pages/).

## GitLab CI/CD

This project's static Pages are built by [GitLab CI/CD](https://about.gitlab.com/stages-devops-lifecycle/continuous-integration/),
following the steps defined in [`.gitlab-ci.yml`](.gitlab-ci.yml).

## Building locally

To work locally with this project, you'll have to follow the steps below:

1. Fork, clone or download this project.
1. Install `git` and `go`.
1. [Install](https://gohugo.io/getting-started/installing/) Hugo.
1. Install the theme as a Hugo module:

   ```shell
   hugo mod init gitlab.com/pages/hugo
   hugo mod get -u github.com/theNewDynamic/gohugo-theme-ananke
   ```

1. Preview your project:

   ```shell
   hugo server
   ```

1. Add content.
1. Optional. Generate the website:

   ```shell
   hugo
   ```

Read more at Hugo's [documentation](https://gohugo.io/getting-started/).

## Use a custom theme

Hugo supports a variety of themes.

Visit <https://themes.gohugo.io/> and pick the theme you want to use. In the
Pages example, we use <https://themes.gohugo.io/themes/gohugo-theme-ananke/>.

### Use a custom theme using a Hugo module

The example [`.gitlab-ci.yml`](.gitlab-ci.yml) uses Hugo modules to import the theme.

To use your own theme:

1. Edit `.gitlab-ci.yml`, and replace the URL in the `hugo mod get` line with the URL of your theme:

   ```yaml
   - hugo mod get -u github.com/theNewDynamic/gohugo-theme-ananke
   ```

1. Edit `config.toml` and add the theme:

   ```plaintext
   theme = ["github.com/theNewDynamic/gohugo-theme-ananke"]
   ```

## `hugo` vs `hugo_extended`

The [Container Registry](https://gitlab.com/pages/hugo/container_registry)
contains two kinds of Hugo Docker images, `hugo` and
`hugo_extended`. Their main difference is that `hugo_extended` comes with
Sass/SCSS support. If you don't know if your theme supports it, it's safe to
use `hugo_extended` since it's a superset of `hugo`.

The Container Registry contains three repositories:

- `registry.gitlab.com/pages/hugo`
- `registry.gitlab.com/pages/hugo/hugo`
- `registry.gitlab.com/pages/hugo/hugo_extended`

`pages/hugo:<version>` and `pages/hugo/hugo:<version>` are effectively the same.
`hugo_extended` was created afterwards, so we had to create the `pages/hugo/` namespace.

See [how the images are built and deployed](https://gitlab.com/pages/hugo/-/blob/707b8e367cdea5dbf471ff5bbec9f684ae51de79/.gitlab-ci.yml#L36-47).

## GitLab User or Group Pages

To use this project as your user/group website, you will need to perform
some additional steps:

1. Rename your project to `namespace.gitlab.io`, where `namespace` is
   your `username` or `groupname`. This can be done by navigating to your
   project's **Settings > General (Advanced)**.
1. Change the `baseurl` setting in your `config.toml`, from `"https://pages.gitlab.io/hugo/"` to `baseurl = "https://namespace.gitlab.io"`.
   Proceed equally if you are using a custom domain: `baseurl = "https://example.com"`.

Read more about [GitLab Pages for projects and user/group websites](https://docs.gitlab.com/ce/user/project/pages/getting_started_part_one.html).

## Did you fork this project?

If you forked this project for your own use, please go to your project's
**Settings** and remove the forking relationship, which won't be necessary
unless you want to contribute back to the upstream project.

## Troubleshooting

### CSS is missing! That means two things:

- Either that you have wrongly set up the CSS URL in your templates.
- Or your static generator has a configuration option that needs to be explicitly
  set in order to serve static assets under a relative URL.

### Hugo fails to build the website

If the version of `hugo` or `hugo_extended` is 0.92.2 or later, you may have problems building the website.

Generics were introduced in [Go 1.18](https://go.dev/blog/go1.18), and they broke some features in the newer versions of Hugo. For now, if you use `hugo` or `hugo_extended` versions 0.92.2 or later, you might encounter problems building the website. To resolve the problem:

1. Edit your `.gitlab-ci.yaml` file.
1. Identify the line that declares the Hugo version.
1. Change the value to `:0.92.2`.
1. Save your changes

For more information about this issue:

- This issue is tracked in [Gitlab Hugo template fails CI/CD build with "latest" docker version](https://gitlab.com/pages/hugo/-/issues/69).
- For discussions about fixing the problem in Hugo, and proposals to potentially resolve these issues, read [proposal: spec: allow type parameters in methods](https://github.com/golang/go/issues/49085).
>>>>>>> upstream/main
