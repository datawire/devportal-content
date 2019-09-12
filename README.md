# devportal-content
User content for Ambassador Pro Dev Portal

## How to customize

- Fork this repository

- Update APRO_DEVPORTAL_CONTENT_URL environment variable in `env.sh` of your
  https://github.com/datawire/pro-ref-arch checkout that you used to install the
  Ambassador Pro

- Run `make apply-ambassador` again

- Modify your fork. Note: for now it's necessary to restart ambassador to
  refresh the portal content. We'll fix this in the next release.

## kinds of content

Kinds of information you can put on dev portal:

| Kind               | Location                       | Preprocessing | Go templates |
|--------------------|--------------------------------|---------------|--------------|
| landing page       | `/landing.gomd`                | Markdown      | Yes          |
| page               | `/pages/`_name_`.gomd`         | Markdown      | Yes          |
| site layout        | `/layout.gohtml`               |               | Yes          |
| template fragments | `/fragments/`_name_`.gohtml`   |               | Yes          |
| CSS stylesheets    | `/styles/`                     |               | No           |
| Assets             | `/assets/`                     |               | No           |

