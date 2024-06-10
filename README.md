# Issue Reproduction

1. Deploy the repository, check the `/opengraph-image.jpg` path.
2. Change the `opengraph-image.jpg` and commit to generate a new deployment.
3. Check the `/opengraph-image.jpg` path - **it will be stale and not have updated**, this applies to production, custom, and system generated URLs.
4. Use **Redeploy** on the latest production deployment from the dashboard and check the `/opengraph-image.jpg` path - you will find the image has now updated.

![CleanShot 2024-06-10 at 09 27 13@2x](https://github.com/mcsdevv/nextjs-og-test/assets/26944716/292c01d3-0524-48d6-9083-657aea87ee0b)
