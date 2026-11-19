# napboo-site

Napboo's public pages: the home page and the account-deletion page that Google
Play and the App Store ask for. Plain HTML and one stylesheet in `public/`, with
no build step, no scripts, and no fonts or trackers from anywhere else.

- `public/index.html`: home
- `public/delete-account.html`: how to delete an account, and what is deleted
  (served at `/delete-account`)
- `public/404.html`: page not found

**Hosting.** Cloudflare Pages builds this repository on every push to `main`
(framework preset None, no build command, output directory `public`) and serves
the same pages on two domains:

- `napboo.co.uk` for the UK;
- `napboo.com` for the US and everywhere else.

Each page names both versions with `hreflang` (`en-GB` for napboo.co.uk, `en`
and `x-default` for napboo.com), so search engines show the right domain. Nobody
is redirected by country. `www.` on either domain redirects to the bare domain.

The privacy policy is drafted in the app's repository
(`flutter-apps/apps/Napboo/store/privacy-policy.html`) and is added here only
once it has been reviewed. The app's code lives in `flutter-apps`
(`apps/Napboo`) and its database in `platform-db`.
