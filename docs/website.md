# Website development

## Writing a blog post

Add a Markdown file in `src/content/blog/`.
Each post needs `title`, `description`, `date` in YYYY-MM-DD format, and `draft` in its frontmatter.
Set `draft: false` to publish. The filename becomes the URL, for example `first-post.md` becomes `/blog/first-post/`.
Published posts appear automatically on `/blog/` and the latest three appear on the homepage. Drafts have no public route.
Start the post body with a paragraph or `##` heading. The page supplies the post title as its only `h1`.
Run `bun run build` after editing content.

## Domains and projects

Edit `domains` in `src/data/site.ts` to add a domain with a name, description, and `href`.
Edit `projects` in the same file to add a project with a name, description, GitHub URL, and optional product link.
Domains and projects appear together on `/projects/`, with domains first. Projects also appear as a compact list on the homepage.
