# Blog Workflow

## Create New Post

```powershell
hugo new content/posts/post-title.md
```

Edit the file in `content/posts/post-title.md`. Set `draft: false` when ready to publish.

## Preview Locally

```powershell
hugo server -D
```

View at http://localhost:1313 (includes drafts with `-D` flag)

## Publish

```powershell
git add .
git commit -m "Add post: title"
git push
```

Live at https://jamesishere.github.io/ within ~60 seconds.

## Post Frontmatter Template

```markdown
---
title: "Post Title"
date: 2024-11-23T10:00:00-05:00
draft: false
---
```

## Common Tasks

| Task                     | Command                                      |
| ------------------------ | -------------------------------------------- |
| New post                 | `hugo new content/posts/slug.md`             |
| Preview (with drafts)    | `hugo server -D`                             |
| Preview (published only) | `hugo server`                                |
| Build static site        | `hugo`                                       |
| Publish                  | `git add . && git commit -m "msg" && git push` |
| Check git status         | `git status`                                 |
| View commit history      | `git log --oneline`                          |

## URL Structure

Posts use date-based URLs: `/YYYY/MM/post-title/`

Example: A post dated 2024-11-23 with title "My First Post" becomes `/2024/11/my-first-post/`
