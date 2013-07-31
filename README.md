google-api-php-client
=====================

#PHP Google API Library

Raison de etre for this version of the google-api-php-client library is to fix bugs in examples folder for AdSense and Analytics, and elsewhere.

##Quickstart
###API Client ID
From the API Access Menu click on "Create anoher client ID..." and configure access for the application type "Web application".

###Simple API Access
From Simple API Access click on "Create new Server key..." and configure accordingly.

AdSenseAuth.php OAuth credentials configuration:
    $this->apiClient->setClientId('<client id from web application>');
    $this->apiClient->setClientSecret('<client secret from web applications >');

    $this->apiClient->setDeveloperKey('<api key from key for server apps under Simple API Access>');
    $this->apiClient->setRedirectUri('<url to>google-api-php-client/examples/adsense');

google-api-php-client/adsense/index.php adsense client configuration:

    define('AD_CLIENT_ID', '<adsense publisher id>');

    define('ACCOUNT_ID', '<adsense account id>');

    define('CUSTOM_CHANNEL_ID', '<adsense channel>');
