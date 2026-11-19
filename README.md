# napboo-site

The public pages for Napboo at https://napboo.com: the home page and the
account-deletion page that Google Play and the App Store ask for. Plain HTML
and one stylesheet, served by GitHub Pages from `main` (root). No scripts, no
fonts or trackers from anywhere else.

- `index.html`: home
- `delete-account.html`: how to delete an account, and what is deleted
- `404.html`: page not found
- `CNAME`: the custom domain (napboo.com)

The privacy policy is drafted in the app's repo
(`flutter-apps/apps/Napboo/store/privacy-policy.html`) and is added here only
once it has been reviewed. The app's code lives in `flutter-apps`
(`apps/Napboo`); its database in `platform-db`.

DNS is on Cloudflare: `napboo.com` points at GitHub Pages and `napboo.co.uk`
redirects to it.
