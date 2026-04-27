# GitHub setup steps for LCMB Smart Quotes

## 1. Create a GitHub account

Create a GitHub account using a business email address.

Suggested usernames:
- `lcmbgroup`
- `lcmbelectrical`
- `lcmbquotes`
- `lcmbelectricalquotes`

If the exact name is not available, use a close version.

Do not send your GitHub password to anyone.

## 2. Create the repository

Create a new repository called:

```text
lcmb-smart-quotes
```

For the first version, choose a public repository if you are using the free GitHub Pages setup.

## 3. Upload these files

Upload everything from this folder to the repository root.

The top level of the repository should look like:

```text
assets/
quotes/
index.html
quote-generator.html
README.md
prompt.md
robots.txt
.nojekyll
GITHUB_SETUP_STEPS.md
SERVICE_M8_TO_QUOTE_WORKFLOW.md
EMAIL_SMS_TEMPLATES.md
QUOTE_CHECKLIST.md
```

Do not upload the ZIP file itself. Upload the files and folders inside it.

## 4. Turn on GitHub Pages

In the repository:

1. Open **Settings**.
2. Open **Pages**.
3. Choose **Deploy from a branch**.
4. Choose branch **main**.
5. Choose folder **/root**.
6. Save.

Wait a few minutes for GitHub to publish the site.

Your first URL will look like:

```text
https://YOUR-GITHUB-USERNAME.github.io/lcmb-smart-quotes/
```

The quote generator will be:

```text
https://YOUR-GITHUB-USERNAME.github.io/lcmb-smart-quotes/quote-generator.html
```

The example quote will be:

```text
https://YOUR-GITHUB-USERNAME.github.io/lcmb-smart-quotes/quotes/example-quote.html
```

## 5. Create a new quote page

1. Open the quote generator.
2. Fill in the ServiceM8/GHL quote details.
3. Click **Preview Quote Page**.
4. Click **Download Quote HTML**.
5. Upload the downloaded file into the `/quotes` folder in GitHub.
6. Copy the live quote URL.
7. Send the link to the customer through ServiceM8 or GHL.

## 6. Future custom domain

Later, set up:

```text
quotes.lcmbgroup.com.au
```

When ready:
1. Rename `CNAME.example` to `CNAME`.
2. Put this inside the file:

```text
quotes.lcmbgroup.com.au
```

3. Add the matching DNS CNAME record with your domain provider.
4. Add the custom domain inside GitHub Pages settings.
5. Wait for DNS and HTTPS to activate.
