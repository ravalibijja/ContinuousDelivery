---

copyright:
  years: 2018
lastupdated: "2018-4-12"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Managing personal data in Continuous Delivery
{: #cd_personal_data}

You can modify, export, or delete personal data from {{site.data.keyword.contdelivery_full}}.
{: shortdesc}

Personal data is any information that relates to or identifies a natural person. For example, personal data can be a name, email address, avatar, token, or any number of identifiers that are used with {{site.data.keyword.contdelivery_short}}. The following {{site.data.keyword.contdelivery_short}} components contain personal data:

 * The Eclipse Orion {{site.data.keyword.webide}}
 * {{site.data.keyword.gitrepos}}
 * {{site.data.keyword.contdelivery_short}} Pipelines
 * Toolchains and tool integrations
 * [GitHub Enterprise on IBM Cloud ![External link icon](../../icons/launch-glyph.svg "External link icon")](/docs/services/ghededicated/ghe_personal_data.html){: new_window}
 * [{{site.data.keyword.DRA_full}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](/docs/services/DevOpsInsights/insights_personal_data.html){: new_window}
 
{{site.data.keyword.contdelivery_short}} provides the appropriate permissions to manage data within a Cloud Foundry organization. Your company might have policies that limit these permissions. If you don't have the appropriate permissions, contact your organization's administrator.

To manage your personal data, you must understand IBM Cloud accounts, how these accounts are used, and their associated access rights.
 
## Accounts and access rights
{: #accounts_access_rights}

To work in IBM Cloud, you must log in with a user name and password. When you log in, IBM Cloud associates at least one IBM Cloud account with your user credentials. When you create resources such as Cloud Foundry organizations and {{site.data.keyword.contdelivery_short}} objects, they are associated with an IBM Cloud account.

The IBM Cloud login structure provides you with the option to work in different accounts. Using the IBM Cloud user interface, you can switch from one account to another. When you log in, any of the following types of accounts might be associated with your user credentials: 

 * Personal account
 * Corporate account
 * Corporate individual account

###Personal accounts

Typically, each user has their own account that is their personal account. You can easily identify your personal account because it usually contains your name, for example, *John Smith's Account*. 

You have full rights over all objects that are created in your personal account. You can invite other users to join your account, assign them rights over objects that you create, and assign them rights to create objects in your account. This means that the personal data of other users might be in your account, and your personal data might be in other user's accounts. 

If you have permission to create an object in an account, you also have the right to modify and delete it, regardless of which account the object is stored in. When two users collaborate, they often share a personal account.

###Corporate accounts

A corporate account is set up by your company. Typically, you are added automatically to the account, rather than being invited. Corporate accounts provide users with a place to work, communicate, and share resources and charging; however, this is just a convention. A corporate account is really no different than a personal account. Objects that are created in a corporate account are associated with the account and users can be invited to the account.

Teams of people who work for a corporation often collaborate using a corporate account.

###Corporate individual accounts

When you work for a corporation, the work in your account might be legally owned by the corporation. Many users who work for a corporation have a corporate individual account. If you log in to your account using credentials that contain your corporation's name and also have what appears to be a personal account, the work within your personal account might belong to the corporation.

A corporate individual account is no different from any other account. You can invite users to a corporate individual account and objects that are created in a corporate individual account are owned by the account.

If you work for a corporation that owns your work, a personal account that usually contains your name is considered a corporate individual account. 

## Modifying, exporting, and deleting personal data
{: #managing_personal_data}

Regardless of what type of IBM Cloud account is used, if you have rights to the objects in the account, you can modify, export, and delete them. Before you make changes, coordinate with other users to make sure that you don't unecessarily modify or delete data.

Before you delete data from an account, determine whether it is a personal account or a corporate individual account.

###Personal accounts

If you own a personal account, you can make changes and delete your data. If you share your account with another user, you own the data, but you might want to contact them about the shared work. 

If you can't log in to your IBM Cloud account, [contact IBM Support ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/cloud/support){:new_window}
 
###Corporate individual accounts

If you own a corporate individual account, you must coordinate any changes with both your corporation and other members of your team. Delete your personal data regardless of whether it is stored in a corporate account or a corporate individual account. Make sure that you don't delete work that you shared with other users.

Before you start to manage your personal data for the {{site.data.keyword.contdelivery_short}} components, make sure that you are working in your IBM Cloud account. To view the IBM Cloud account that you are currently working in, on the menu bar, click your profile avatar. 

If you can't log in to your IBM Cloud account, contact your corporation and work with them to delete your personal data.

**Important**: If you want to delete all of your personal data from {{site.data.keyword.contdelivery_short}}, the order in which you delete that data is important. First, delete all of your {{site.data.keyword.webide}} workspaces, next delete your {{site.data.keyword.gitrepos}} data, and then delete your {{site.data.keyword.gitrepos}} account. Finally, delete your delivery pipelines, tool integrations, and toolchains.

## Exporting and deleting Web IDE data
{: #managing_web_ide_data}

The {{site.data.keyword.webide}} provides a personal workspace in the cloud. You can use the {{site.data.keyword.webide}} to clone Git repositories and edit files. You own your {{site.data.keyword.webide}} workspace; it is not shared by any other account.

**Tip**: Before you delete your {{site.data.keyword.webide}} data, you might want to export your work. After you delete your workspaces, they are removed from {{site.data.keyword.contdelivery_short}} and all files are deleted.

###Exporting a Web IDE workspace

To export a {{site.data.keyword.webide}} workspace:

1. Select **File > Export > Zip**.
1. Repeat for each workspace that you want to export.

###Deleting your Web IDE workspaces

To delete your {{site.data.keyword.webide}} workspaces, including all of your personal data:

1. From any toolchain, navigate to the {{site.data.keyword.webide}}.
1. Click the **Settings** icon <img class="inline" src="images/webide_settings_icon_light_small.png"  alt="The settings icon"> in the navigation sidebar on the left.
1. Click **USER PROFILE**.
1. Click **Delete** to remove all of your data from the {{site.data.keyword.webide}}.

**Important**: The {{site.data.keyword.webide}} uses a single sign-on mechanism. The first time that you access this tool integration, a corresponding, but hidden, {{site.data.keyword.webide}} account is created for your IBM Cloud account. After you delete all of your workspaces, do not access the {{site.data.keyword.webide}}. If you access the {{site.data.keyword.webide}} again, a new account is automatically created that you must delete.

## Modifying, exporting, and deleting Git Repos and Issue Tracking data
{: #managing_grit_data}

{{site.data.keyword.gitrepos}} provides a hosted Git service in the cloud. A single sign-on mechanism is used to associate your IBM Cloud account with a Git account. A full name and a short name are created for you in your Git account. Other users can use your short name to refer to you in a comment within a Git issue. You can customize your Git account and add personal data such as a description of yourself or an image. 

{{site.data.keyword.gitrepos}} provides a powerful, but complex social coding environment in which users contribute to different projects and objects are shared. This environment can make it difficult to locate and delete your personal data.

Your account profiles and settings, personal projects, groups, and snippets are associated with your Git account. If you delete your Git account, these objects are deleted. To delete personal data in another project, navigate to the project, and then modify it to remove your personal data, or delete the project entirely. Make sure that you coordinate with other members of your team before you delete shared projects.

**Important**: Before you delete your Git account, delete your personal data from other projects. After you delete your Git account, it might be difficult or impossible to find all of the projects that you contributed to.

###Personal and shared projects

You can invite other users to collaborate in projects. Git projects that you create inside your account are called personal projects. You can also create Git groups in which projects can be owned by multiple Git owners. You can create new projects for the group or transfer ownership of personal projects to the group. A Git group is often used to represent an IBM Cloud corporate account to indicate ownership of projects by the corporation.

###Exporting a Git Repos and Issue Tracking project

Before you delete a {{site.data.keyword.gitrepos}} project, you can export the project to archive it. 

1. Click the **Settings** icon <img class="inline" src="images/webide_settings_icon_light_small.png"  alt="The settings icon"> in the navigation sidebar on the left.
1. Click **General**.
1. Click **Expand** to expand the Export project section.
1. Click **Export project**.

After the project is archived, you can import it into another GitLab instance. 

###Deleting your Git Repos and Issue Tracking account

You can delete your {{site.data.keyword.gitrepos}} account and everything that is owned by that account.

1. On the {{site.data.keyword.gitrepos}} User Settings dashboard, on the [Account page ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://git.ng.bluemix.net/profile/account?cm_sp=dw-bluemix-_-nospace-_-answers){:new_window}, in the Delete account section, click **Delete account**.
1. All Git projects, including repositories and issues are deleted. You are also removed from any {{site.data.keyword.gitrepos}} groups that you belong to.

**Tip**: After your account is deleted, some content will remain. This content is assigned to a system wide Ghost User. For more information about deleting a {{site.data.keyword.gitrepos}} account, see [Deleting a user account ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://git.ng.bluemix.net/profile/account/delete_account#associated-records){:new_window}.

**Important**: {{site.data.keyword.gitrepos}} uses a single sign-on mechanism that automatically creates a corresponding Git account for your IBM Cloud account the first time that you access the tool integration. After you delete your account, do not access {{site.data.keyword.gitrepos}}. If you access {{site.data.keyword.gitrepos}} again, a new account is automatically created that you must delete.

## Modifying and deleting Continuous Delivery pipeline data
{: #managing_pipeline_data}

{{site.data.keyword.contdelivery_short}} pipelines run scripts to build, test, and deploy your application to the IBM Cloud. To do this, pipelines provide stages, jobs, environment variables, and other objects that might contain personal data. You can delete these objects individually or you can delete an entire pipeline.

Make sure that you coordinate with other members of your team before you delete shared objects or pipelines. Deleting a stage might cause a pipeline to fail.

**Tip**: A pipeline cannot exist outside of a toolchain. If you delete a toolchain, all of the pipelines that are associated with the toolchain are also deleted. If you plan to delete an entire toolchain, you do not need to delete each pipeline individually. Instead, skip to the "Modifying and deleting toolchains and tool integrations" section, and follow the steps to delete a toolchain.

###Modifying and deleting pipeline stages

Pipeline stages might include personal data such as credentials in the form of environment properties. Stages might also include scripts inside jobs that you want to modify or delete. Use the Configure Stage or Delete Stage actions to modify or delete a stage.

  ![Stages menu](images/pipeline_stages.png)

To modify a pipeline stage:

1. On the Pipeline page, click the **Settings** icon.
1. Click **Configure Stage**.
1. On the **ENVIRONMENT PROPERTIES** tab, edit or delete properties.
1. Modify a job script within the pipeline stage. Select the job and change the values that are part of the Build, Deploy, or Test Configuration.
   
   ![Modify job script](images/job_script.png)
  
1. Delete a job from the pipeline stage. On the **JOBS** tab, select the job that you want to delete and click **Remove**.
 
To delete a pipeline stage:

1. On the Pipeline page, click the **Settings** icon.
1. Click **Delete Stage**.

###Changing pipeline ownership

You can transfer ownership of a pipeline that you own to another user; the new owner must perform the transfer operation. A user can take ownership of an existing pipeline, but they cannot assign ownership to another user. You must have ADMIN rights to take ownership of a pipeline.

To take ownership of a pipeline, a user must complete the following steps:

1. Log in to IBM Cloud.
1. Click the menu to access the configuration options. 

  ![Configuration menu](images/pipeline_ownership.png)

1. Click **Modify Pipeline Owner**. 
1. Select **MAKE ME OWNER**.

## Modifying and deleting toolchains and tool integrations
{: #managing_toolchains}

By using toolchains, teams can collaborate and and share different tool integrations. 

It is recommended that you configure all {{site.data.keyword.contdelivery_short}} integrations by using data that is associated with your team or company, rather than data that is associated with you. However, there might be instances where your personal data is inadvertently used instead. In such instances, you must identify all of the data that you own and delete it.

When a tool integration is created, {{site.data.keyword.contdelivery_short}} cannot record the origin of all of the data. For example, another team member might create a tool integration for you by using personal data that you provide in an email. You must understand which data you own and make sure that it is deleted.

Coordinate with other members of your team before you delete shared tool integrations or toolchains.

###Modifying and deleting tool integrations

When you create a tool integration, you are required to provide user credentials and other account information that pertains to the integration. If you used your own personal credentials and account information, replace this information with different values, or delete the tool integration.

To modify a tool integration:

1. On the tool's card, click the menu to access the configuration options.

  ![Tool Configuration menu](images/toolchain_tile_menu.png)

1. When you are finished updating the settings, click **Save Integration**.

To delete a tool integration:

1. To delete a tool integration from your toolchain, click **Delete**.
1. Confirm by clicking **Delete**.


###Deleting toolchains

When you delete a toolchain, the deletion cannot be undone.

1. On the DevOps dashboard, on the **Toolchains** page, click the toolchain to delete. Alternatively, on the app's Overview page, on the Continuous delivery card, click **View Toolchain**.
1. Click the **More Actions** menu, which is next to **View app**.
1. Click **Delete**. Deleting a toolchain removes all of its tool integrations, including pipelines, which might delete resources that are managed by those integrations.
1. Confirm the deletion by typing the name of the toolchain and clicking **Delete**. 

###Deleting all toolchains

You cannot delete all of the toolchains within an organization at the same time. You must delete each toolchain, one at a time.

**Important**: Toolchains are scoped by IBM Cloud region and Cloud Foundry organization. Make sure that you select each region and organization within the region to delete every toolchain that you created.