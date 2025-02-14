---
title: Making a GitHub App public or private
intro: '{% data reusables.shortdesc.making-a-github-app-public-or-private %}'
redirect_from:
  - /apps/building-integrations/setting-up-and-registering-github-apps/about-installation-options-for-github-apps
  - /apps/building-github-apps/installation-options-for-github-apps
  - /apps/building-integrations/managing-github-apps/changing-a-github-app-s-installation-option
  - /apps/managing-github-apps/changing-a-github-app-s-installation-option
  - /apps/managing-github-apps/making-a-github-app-public-or-private
  - /developers/apps/making-a-github-app-public-or-private
  - /developers/apps/managing-github-apps/making-a-github-app-public-or-private
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - GitHub Apps
shortTitle: Manage app visibility
---
For authentication information, see "[AUTOTITLE](/apps/creating-github-apps/authenticating-with-a-github-app/authenticating-with-github-apps#authenticating-as-an-installation)."

## Public installation flow

Public installation flows have a landing page to enable other people besides the app owner to install the app in their repositories. This link is provided in the "Public link" field when setting up your GitHub App. For more information, see "[AUTOTITLE](/apps/maintaining-github-apps/installing-github-apps)."

## Private installation flow

Private installation flows allow only the owner of a GitHub App to install it. Limited information about the GitHub App will still exist on a public page, but the **Install** button will only be available to organization administrators or the personal account if the GitHub App is owned by an individual account. Private GitHub Apps can only be installed on the user or organization account of the owner.

## Changing who can install your GitHub App

To change who can install the GitHub App:

{% data reusables.user-settings.access_settings %}
{% data reusables.user-settings.developer_settings %}
{% data reusables.user-settings.github_apps %}
3. Select the GitHub App whose installation option you want to change.
{% data reusables.user-settings.github_apps_advanced %}
5. Depending on the installation option of your GitHub App, click either **Make public** or **Make private**.
6. Depending on the installation option of your GitHub App, click either **Yes, make this GitHub App public** or **Yes, make this GitHub App {% ifversion fpt or ghec %}internal{% else %}private{% endif %}**.
