# Supabase Snippets for Visual Studio Code

Supabase Snippets is a Visual Studio Code extension that provides handy snippets for working with the Supabase.io platform. These snippets allow developers to quickly generate code for common Supabase operations, saving time and reducing errors.

## Features

This extension includes the following snippets:

| Snippet | Description |
|---------|-------------|
| `sbs`   | Generates a Supabase select query. |
| `sbi`   | Generates a Supabase insert query. |
| `sbu`   | Generates a Supabase update query. |
| `sbsr`  | Generates a Supabase search query. |
| `sbd`   | Generates a Supabase delete query. |

## Usage

To use a snippet, simply type its prefix in a JavaScript or TypeScript file and press `Tab` to expand it. Fill in any placeholders as needed.

For example, typing `sbs` and pressing `Tab` will expand to:

```javascript
const { data, error } = await supabase
    .from('$1')
    .select(`$2`)

if (error) {
    throw new Error(error.details)
}
return data;
