# Example

A small plugin that uses every part of Lerd a plugin can add, so you can see each one working before you write your own. Nothing here changes your sites.

## What to try

- **Terminal**: `lerd example:greet [site]` prints a greeting for a site; `lerd example:sites` lists your sites through Lerd's own API.
- **Commands menu**: every site gets **Greet**, which runs the same greeting.
- **Rail page**: the **Example** page on the dashboard's rail asks for a site name and greets it through the plugin's own API endpoint.
- **Site tab**: every site gets an **Example** tab that greets the site it is opened on.
- **Overview card**: switch it on from the plugin icon in a site's header, and the site's Overview gets a small Example card.
- **Page script**: switch it on the same way, or with `lerd plugin page example on` in the project, and the site's own pages get a small button that calls the plugin.
- **Hooks**: linking or unlinking a site appends the event to `events.log` in the plugin's data folder.
- **AI assistants**: `example_greet` through Lerd's MCP server, with a skill saying when to use it.

## Make your own

```bash
lerd plugin new my-plugin
```

starts from this same plugin under your own name. Delete what you do not need, write your docs in its DOCS.md, and read the plugin guide at lerd.sh/features/plugins.
