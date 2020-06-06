# [chest.store](https://chest.store) Marketing Website

## Original Template

https://github.com/BlackrockDigital/startbootstrap-grayscale

## Deployment

chest.store's website is deployed to AWS S3 as a static site. Use the
following instructions to deploy after changes have been make.

### macOS

1. Make sure AWS CLI is installed via [Homebrew](https://brew.sh/)
    - `brew install awscli`
2. After changes are made, build to `dist`
    - `npm run build`
3. `aws s3 cp --recursive dist s3://chest.store`
4. Clear cloudfront distribution cache (via UI today, TODO instructions via CLI)
