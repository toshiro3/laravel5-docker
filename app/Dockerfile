FROM _AWS_ACCOUNT_ID_.dkr.ecr._AWS_DEFAULT_REGION_.amazonaws.com/_IMAGE_REPO_NAME_:_IMAGE_TAG_

ADD laravel5-sample /var/www/app/

WORKDIR /var/www/app
EXPOSE 9000
CMD ["php", "artisan", "serve", "--host", "0.0.0.0", "--port", "9000"]
