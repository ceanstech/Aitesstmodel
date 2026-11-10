<<<<<<< ours
<<<<<<< ours
<<<<<<< ours
This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
=======
=======
>>>>>>> theirs
=======
>>>>>>> theirs
# Hmong Dictionary Importer

A small command-line tool for preparing a Hmong dictionary before saving it to a database.

The importer reads a CSV file, groups entries by the first alphabetical letter (`A`, `B`, `C`, ...), sorts words inside each group, and stores the result in SQLite.

## CSV format

```csv
word,meaning,pronunciation,example
ab,older sibling,,, 
aj,what,,
ca,branch,,
```

Only `word` and `meaning` are required. `pronunciation` and `example` are optional.

## Usage

```bash
python3 hmong_dictionary_importer.py words.csv hmong_dictionary.db
```

Print grouped preview without writing a database:

```bash
python3 hmong_dictionary_importer.py words.csv --dry-run
```

## Database schema

The tool creates an `entries` table with these columns:

- `id`
- `letter`
- `word`
- `meaning`
- `pronunciation`
- `example`
- `sort_key`

The `letter` column stores the alphabet group so the app can show dictionary sections such as `A`, `B`, and `C`.
<<<<<<< ours
<<<<<<< ours
>>>>>>> theirs
=======
>>>>>>> theirs
=======
>>>>>>> theirs
