# devportal-content
User content for Ambassador Edge Stack Dev Portal

## How to customize

- Fork this repository.

- Update the `DEVPORTAL_CONTENT_URL` environment variable in your Ambassador Edge Stack deployment.

- Modify your fork. Note: for now it's necessary to restart ambassador to refresh the portal content. We'll fix this in the next release.

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
