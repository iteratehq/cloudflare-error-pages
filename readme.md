# Iterate Cloudflare Error Pages

Custom branded error pages for Cloudflare 500 class errors.

Cloudflare allows for custom branded error pages to help provide a consistent brand experience for our users. These pages can have custom html, css, and assets. The total page weight should be less than 1.43MB, and must include the `::CLOUDFLARE_ERROR_500S_BOX::` token.

![Iterate's Cloudflare Error page](https://iterate-assets.s3.amazonaws.com/errorpage/iterate-errorpage.png)

## Deploying changes

1. Upload the updated changes to S3.
2. Grant public read access to the file.
3. In Cloudflare's Custom Pages UI, select **Edit** for the 500/1000 Class errors. Paste the new S3 URL, select **Preview** & confirm Cloudflare sees the page as valid. Publish the new page.

## Resources

- Cloudflare: [Configuring Custom Pages (Error and Challenge)](https://support.cloudflare.com/hc/en-us/articles/200172706-Configuring-Custom-Pages-Error-and-Challenge-)
- Inspiration: [Artsy Cloudflare Error Pages](https://github.com/artsy/cloudflare-error-pages/blob/main/README.md)
