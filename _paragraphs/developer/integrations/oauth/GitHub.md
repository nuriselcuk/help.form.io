---
title: Github
book: developer
section: integrations
chapter: oauth
slug: github
weight: 10
---
Login to GitHub and visit your [Developer applications settings page](https://github.com/settings/developers).

Click *Register new application*.

Fill in the Application name, Homepage URL, and Application description with appropriate details about your application. This information is displayed to potential users of your application when they asked to grant permissions to your app.

Fill in the **Authorization callback URL** with your application's **hostname**. OAuth will not work unless you enter the same hostname as the one your application is served from. Using `localhost` for running your app locally is acceptable, but make sure the right port is provided.

![](/assets/img/oauth/github-app-settings-edit.png)

Click *Register application*.

Take note of the Client ID and Client Secret. Enter them in the Project Settings for GitHub Oauth.

![](/assets/img/oauth/github-app-settings-view.png)

Github OAuth should now be set up. Continue with adding [Login, Register and Link buttons](#button) to your forms.
