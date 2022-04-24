 <!-- Title, author, date block standard in all files -->
# Blog editorial process - from idea to published
<!-- Commented out so it doesn't render to webpage
----
*Author(s): @quaid*<br/>
*Date Created: 2022-04-24*<br/>
*Date Updated: N/A or YYYY-MM-DD*<br/>
*Status: DRAFT*<br/>
----
-->
<!-- Brief description standard in all files -->
**This document describes the process to go from an idea to a published blog post, describing the steps on the [editorial workflow board](TBD).**

## Blog idea (Owner: Writers)

When you have an idea for a blog post — no matter how incomplete the idea is — open and fill out an issue template that puts your card into the beginning of the editorial process.
This is how you can propose and discuss a blog post idea before you begin drafting the post.
This can be helpful for developing your idea before you get too far into the writing process.

1. Go to the [issues page in the `blog` repo](https://github.com/operate-first/blog/issues) and choose the ["New Blog Post" template](TBD).
1. Fill out the template, replacing the _italicized instructions_ with your information or answers.
1. Submit the issue, which puts it in the queue of blog ideas.
1. If you are in contact with an [editor](TBD), you can let them know the idea has been submitted.
 Otherwise, an editor will contact you, typically within 72 hours (not including weekends.)

## Blog draft (Owner: Writers)

TBD: write out all the GitHub UI steps; provide actual links for the TBD links.

When you have a draft for a blog post, you will open a pull request with the blog post as a MarkDown file.

This section presumes you are familiar with the [Op1st process for making a pull request](TBD) and are prepared to provide the blog post using a [provided MarkDown template](TBD).

> :bulb: **Tip** These steps are intended to be useful to a novice user, but you are not alone if you get stuck and need help.
You can seek help from anyone in the community in the [#support channel on Slack](TBD).

> :notebook: **Note** This section includes instructions for using the GitHub UI, and does not provide directions for using `git` on the command line locally.
Help and recommended reading for that can be found in the [Op1st Community Handbook section on git](TBD).

1. If you don't already have your own fork, fork the `blog` repo to your personal GitHub space.
1. In your fork (or clone, if you are working locally) create a new branch for this blog post, such as `short-version-post-title`.
 Working in a branch for each blog post makes it possible to have more than one post in the editorial process at the same time.
1. In the `content/subsection/` where your post belongs, make a copy of the `docs/blog-post-template.md` file.
1. Open that file for editing, replacing the content of the template with your blog post.
 Use the visual renderer built-in to GitHub to check your MarkDown for errors.
1. When you are satisfied with the draft in MarkDown, save and commit the file.
1. Returning to the [main blog repo](https://github.com/operate-first/blog), you will see the suggestion to make a pull request, which you can do.
1. Fill out any needed parts of the pull request, then complete and submit it.

If your blog post PR is associated with an idea discussed in an issue, an editor may tie this PR to close out that issue when the blog post is merged (published).

## Blog review (Owner: Reviewers)

_Reviewers_ are editors, subject matter experts, other writers, and other community members who are interested in helping improve blog posts before publication.

1. In the GitHub UI for the blog post's pull request, use this [process for commenting and making suggestions on content in a pull request](TBD).
1. Use the **Review** button to create your review, choosing one of **Approve**, **Request Changes**, or **Comment**.
You can make further reviews after changes have been made, if you wish.
1. When you are finished with your review, note your approval by adding the command `/lgtm` on a line by itself in a __Comment__ in the pull request.
The post's editor is looking for all reviewers to place the label `lgtm`, which is an acronym for "looks good to me".

Blog posts that are fully approved can be pushed live/pubished to the website by one of the [editors](TBD).

## Blog editing (Owner: Editors)

Editors have two key roles:

1. Helping writers develop, polish, and finish blog posts.
1. Publishing finished posts to the blog.

### Pre-publication editorial - developing, polishing, and finishing posts

1. Idea development - work with writers on ideas proposed, helping them to find the key story to tell and how to tell it.
1. Early draft and helping with clarity - it can be very helpful to work with writers early in the drafting process, especially when the relationship between writer and editor is new.
1. Polishing draft and engaging with SME Reviewers - work with the writers and any necessary reviewers to make sure the reviews happen, including using GitHub tools in the PR to request changes, request reviews, and keep track of `lgtm` labels from various reviewers.
1. Final copyedit - after all factual changes are made, the editors need to go over the blog post for grammar, spelling, punctuation, clarity, and so forth.
 There are two style guides to follow, one for [technical markup style](TBD) and one for [grammar and punctuation](TBD).  

### Publishing finished posts to the blog

1. As the editor of this post, when you are satisfied  it is ready, use GitOps/ChatOps commands to add the `lgtm` label.
1. Use GitOps/ChatOps to approve the finished PR with the `approve` label.
1. Publishing occurs automatically at this point, with any changes to the published post requiring additional pull requests to the file.
