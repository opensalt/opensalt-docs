.. image:: static/OpenSALT_User_Manual_1.png
   :height: 222 px
   :width: 230 px


OpenSALT v.2.2 - User Manual

**Revision History**

+---------+------------+-------+-----------------------+----------------+
|Name     |Organization|Date   |Revision Notes         |Document Version|
+=========+============+=======+=======================+================+
|J Kaufman| PCG        |8/2017 |Original Draft for v1.0|.0              |
+---------+------------+-------+-----------------------+----------------+
|B Dorman | ACT        |11/2017|Updating Import Guide  |.1              |
+---------+------------+-------+-----------------------+----------------+
|J Marks  | PCG        |03/2018|OpenSALT v2.0          |.2              |
+---------+------------+-------+-----------------------+----------------+
|B Dorman | ACT        |05/2018|OpenSALT v2.1          |.3              |
+---------+------------+-------+-----------------------+----------------+
|B Dorman | ACT        |07/2019|OpenSALT v2.2          |.4              |
+---------+------------+-------+-----------------------+----------------+

**Table of Contents**

| `Introduction <#hb79795d3e46b47696c7c5b6d3a41e>`_
| `1.0  Audience <#h1911265d3f1258581a361721a6cd74>`_
| `2.0  OpenSALT Structure and Access <#h787f432939517708191470483c5f43>`_
|     `2.1 OpenSALT Structure <#h5064c4520537f221a7341492e6a4025>`_
|     `2.2 OpenSALT Home Page <#h673d3c62a785f726a6b6333444e4b70>`_
|     `2.3 Log into OpenSALT <#ha586e2f5d293a123c76302e1b7822>`_
|     `2.4 Log off from OpenSALT <#h5b52241c7178667e18023622a381f1>`_
| `3.0  User Roles and Permissions <#h1b685a27e68c571dd1c317e122f34>`_
|     `3.1 Super User <#h155d6d5f4916497a1c6b10341f214165>`_
|     `3.2 Super Editor <#h2b5616331387667a40761f394f7b10>`_
|     `3.3 Organization Admin <#h4e2218295d122347968407129336e50>`_
|     `3.4 Organization Editor <#h223559828a7e63152e784375423e27>`_
|     `3.5 Organization Reviewer <#h5ca4f6060522c494356773e1b9d6>`_
|     `3.6 Public User <#h6047727375e794d1cd6e73641d1357>`_
| `4.0 Organization Management <#h6113256bc274e5e44d234a57614658>`_
|     `4.1 Show Organizations <#h2e38184e3252357f696d5953437a1433>`_
|     `4.2 Add/Create Organization <#h3c64e441156177a1577f6b7b1f6b35>`_
|     `4.3 Edit Organization <#h6e6b6c492a472a26603a601b4348370>`_
|     `4.4 Delete Organization <#h2e57757e4b2674d5e64291645c184>`_
| `5.0  User Management <#h80265f116c6c7b4877762ed5412155>`_
|     `5.1 Change Password <#h6d192e6d564f37133d53288be95d>`_
|     `5.2 Manage Users <#h42723a63d41151f712948537a568079>`_
|         `5.2.1 View User <#hfc27428297e2b766e5a37643a705f>`_
|         `5.2.2 Add/Create User <#h146b5979664d766a2a69263e3512862>`_
|         `5.2.3 Show User <#h6e39602150137e754564a16671b646>`_
|         `5.2.4 Edit User <#h6478147d1f4c85e5d62858217e145d>`_
|         `5.2.5 Suspend User <#h1cf396e28322d368416f6957481b1a>`_
|         `5.2.6 Reinstate User <#h4d2e44565174e175b786376651a7d7c>`_
|         `5.2.7 Delete User <#h3c3329734240281c30b512222591212>`_
| `6.0  Framework Management <#h26624554674c365425514b624a121c24>`_
|     `6.1 Navigate and View Frameworks <#h1c4d1853674733a7f15411e4b788>`_
|         `6.1.1 OpenSalt Home / Contents View Page <#h35526e50752d323810506420224185f>`_
|             `6.1.1.1 Public View <#h1a7c6c1a163f6979313e611a1465218>`_
|             `6.1.1.2 Credentialed View <#h7997a7f1949334b7f84a24785861b>`_
|         `6.1.2 Display Frameworks Page <#h715a2b6d63b2a41b18341215f345f>`_
|             `6.1.2.1 Public View <#h473664e5a545502f3e27165c142d>`_
|             `6.1.2.2 Credentialed View <#hb622c455c38115d3972105a6f2f751e>`_
|             `6.1.2.3 Log View <#hb622c455c38115d3972105a6f2f751f>`_
|          `6.1.3 Adoption Status Security Features <#h473664e5a545502f3e27165c142e>`_
|     `6.2 OpenSALT Frameworks <#h6e1cc76c3a603b3c6b78172573b9>`_
|         `6.2.1 Import Frameworks <#h13a3f4f5767166b3c411a397a2511b>`_
|             `6.2.1.1 Import CASE-Compliant (JSON) File <#h3f23193f6633791f3f387f632bb3d54>`_
|             `6.2.1.2 Import framework from Spreadsheet <#h3f23193f6633791f3f387f632bb3d55>`_
|         `6.2.2  Manually Create Frameworks <#h603062394f35362239624c28149787d>`_
|         `6.2.3 Edit Frameworks <#h2a278644e81e7672704d5078541c5>`_
|         `6.2.4 Delete Frameworks <#ha6bf1778138296b7384e6b3d144c>`_
|         `6.2.5 Update Frameworks from spreadsheet <#h10414a76521969321d1aa7b43555d12>`_
|         `6.2.6 Create new associations via Spreadsheet Update Features <#h405471134e472ab58320531a7c433>`_
|         `6.2.6.1 Update Associations on the same server <#h405471134e472ab58320531a7c444>`_
|         `6.2.6.2 Update Associations from an external server <#h405471134e472ab58320531a7c455>`_
|         `6.2.7 Copy Framework <#h405471134e472ab58320531a7c456>`_
|         `6.2.7.1 Copy Framework only <#h405471134e472ab58320531a7c457>`_
|         `6.2.7.2 Copy entire framework and Make Derivative Framework <#h405471134e472ab58320531a7c458>`_
|     `6.3 Framework Items <#h10414a76521969321d1aa7b43555d10>`_
|         `6.3.1 Import Items with OpenSALT Template <#h8523c2e335f3f114642662c4257c>`_
|             `6.3.1.1 CSV Loading Guide for CASE <#h5777746416576973633711c4a42414c>`_
|             `6.3.1.2 Import Process <#h9291733595a7a78664a32f6e6f6f12>`_
|             `6.3.1.3  Error Log <#h23320351bb10619415c7276b33c>`_
|         `6.3.2 HTML Formatting <#h117048805776102d7a113720452f3f0>`_
|         `6.3.2 Create Items Manually <#h757c75c270717938461c1778456b40>`_
|         `6.3.3 Parent vs Child Items <#hee11494ea5a737422533f4857a34>`_
|         `6.3.4 Edit Items <#h34582e2c50517f447c3367b591218>`_
|             `6.3.4.1 Edit Item Content <#h11415a1c7a7424802ff154b3f2252>`_
|             `6.3.4.2 Edit Item Positions <#h6e264f53772d28c3a845e5e2246>`_
|         `6.3.5 Delete Items <#h1b3dd616c45b553829304021334350>`_
|             `6.3.5.1 Delete Child Item <#h2f4b7d7a715b621354f7a54d243844>`_
|             `6.3.5.2 Delete Parent Item <#h6a5c563e12623b7a81e2b634f8569>`_
|     `6.4 Exemplars for Items <#h417d2d687a6e463a4f2e12321e305c68>`_
|         `6.4.1 Add Exemplar <#h1f2d7057546c742f477446913652e37>`_
|         `6.4.2 Delete Exemplar <#h121a4c79224b7fc925545a2e64286f>`_
|     `6.5 Derivative Frameworks - Copy Items <#h38345071571251147d64497174403132>`_
|     `6.6 Association Management <#h3130761b154e2b57715e7f2385a5548>`_
|         `6.6.1 Associations <#h7529305c281925361d6f9354e774716>`_
|             `6.6.1.1 Create Associations <#h2558124e33f4e6a415f47d675f2742>`_
|             `6.6.1.2 Edit Associations <#h29645036134039768f4f2c4457652d>`_
|             `6.6.1.2 Delete Associations <#h3465b16792e30151f3c47675d20f4c>`_
|                 `6.6.1.2.1 Delete Associations from Tree View <#h1d2176383b1f54c754861c1758301b>`_
|                 `6.6.1.2.2 Delete Associations from Association View <#h111d2e1478713d77723970494749152>`_
|         `6.6.2 Association Groups <#h48482a61264d7437205d1a12f3f3d6b>`_
|         `6.6.3 Crosswalk Associations <#h6fe4164b12672914514d4f13492564>`_
|             `6.6.3.1 Create Crosswalk Associations <#h3123662d575a5b54732475fd62e>`_
|             `6.6.3.2 Edit Crosswalk Associations <#h0571ea6415539114494f5a71425a>`_
|             `6.6.3.3 Delete Crosswalk Associations <#h5d772b55c793e1c441729195453c14>`_
|     `6.7 Export Frameworks Packages <#h4f5432411f2146301151697341562b46>`_
|         `6.7.1 Export Competency Framework Package (JSON) File <#h163e401e8291001a4c5447e45136c>`_
|         `6.7.2 Export Styled PDF (Future Function) <#h69105f5c3a80644f6a806369c586458>`_
|         `6.7.3 Export Spreadsheet <#h596b20112477664e57757b30727b58>`_
|             `6.7.3.1 CF Doc Tab <#h2c3d432f26522266f31614d703c15b>`_
|             `6.7.3.2 CF Item Tab <#h495651a32261e342218226c7b239>`_
|             `6.7.3.3 CF Association Tab <#h7a453f1eb35d645b3d574c4e4a2552>`_
|         `6.7.4 Export HTML Archive (Future Function) <#h637197e5b246b4c3f7c222d352d67>`_
|         `6.7.5 Link for Browser View <#h74c126565a611e731014cb6b8>`_
| `7.0 Options <#h3e237e1a4d5b2d787d76433f407b725f>`_
|     `7.1 Commenting Module <#h366f59222a45735257254b1927547c6a>`_
|         `7.1.2. Features <#h2e1e53322a7678fc1a293916464311>`_
|         `7.1.3 Viewing Comments <#hf2b15673b1ad53c735328544e7e1d>`_
|         `7.1.4 Commenting Configuration <#h5cc5056584c262f761b5b2746a346b>`_
|      `7.2 Automated User Sign up <#h662f65664e775a707382e4d3e1c37>`_
|          `7.2.1 Features <#h5cc5056584c262f761b5b2746a3437>`_
|          `7.2.2 Process <#h5cc5056584c262f761b5b2746a324a>`_
|          `7.2.3 Configuration <#j5cc5056584c262f761b5b2746a346o>`_
|      `7.3 Additional Fields <#j5cc5056584c262f761b5b2746a3460>`_
|      `7.4 File/Image Upload <#j5cc5056584c262f761b5b2746a3461>`_


.. _hb79795d3e46b47696c7c5b6d3a41e:

Introduction
============

**CASE**

CASE establishes a new, global technical standard for the exchange of machine readable, linked data versions of state and national academic standards, local learning objectives and targets, or any workplace, military, or higher education competencies representing skills, knowledge, or abilities. To learn more please visit: \ |LINK1|\

.. |LINK1| raw:: html

    <a href="https://www.imsglobal.org/introduction-case-competencies-and-academic-standards-exchange-case" target="_blank">https://www.imsglobal.org/introduction-case-competencies-and-academic-standards-exchange-case</a>


**OpenSALT**

To support CASE, PCG Education (A national public sector consulting practice); ACT Inc and SchoolCity (both leading curriculum and assessment providers), partnered on the development of the open source project called OpenSALT, that provides a free, IMS-conformance certified tool that enables education organizations to manage and publish frameworks and crosswalks to other standards.

Developed as an open source project, OpenSALT provides for easy exchange of state standards data and provides for and enables alignment services to align educational content to learning standards, as well as correlate (Crosswalk) between different state standards and competency frameworks.


**Key features that distinguish OpenSALT:**

* Easily create derivative frameworks from national standards for use within States

* Create customized competency frameworks with connections to national and state frameworks as needed

* Set learning progressions within a framework

* Allow different views of a framework (For example, view the Standards of Engineering Practices in the NGSS framework separately from the DCI statements)

* Filter frameworks by keyword

* Enabled for the common alignment of resources and assessments to standards

* A Consistent digital format that can be easily integrated into ed-tech products and internal documents alike (Export to the standardized CASE Format as well as spreadsheets)




.. _h1911265d3f1258581a361721a6cd74:

1.0  Audience
=============

This document is intended as a complete guide for using OpenSALT. This document is specially designed for all users with advanced permissions or non-specialists who may find the document useful as a  point of reference. By reading this guide, you will learn how to use OpenSALT through the elements of the graphical user interface (GUI) and explanations of some of the advanced features to provide best practices. This guide will help you to navigate and easily use OpenSALT. The functions and features described in this guide will indicate any role restrictions or limitations as to what users can access or interact with the given system function.

.. _h486792f4a12b6443784e11c1032c:

1.1 Platform Requirements
-------------------------

The user interface is designed using current web standards and supports most modern browsers, in their current supported versions, on a variety of desktop and mobile devices.

The user interface requires JavaScript to be enabled and internet access to be available (no support for an offline mode is currently available).

The user interface should support the latest versions of the following web browsers on desktop and mobile devices:

* Chrome

* Internet Explorer

* Edge

* Safari

* Firefox

.. _h556146c2387114251125619317e27:

2.0  OpenSALT Structure and Access
===================================

OpenSALT is designed to be an open, publicly accessible, framework site that allows transparency in frameworks and crosswalks. By design users are able to traverse and view the published frameworks and content by accessing the main url for the given site. OpenSALT then utilizes a login that allows provisioned users to create, edit and otherwise interact with the frameworks for the site.

.. _h5064c4520537f221a7341492e6a4025:

2.1 OpenSALT Structure
----------------------

OpenSALT goes to the home page by default, and also has a document tree view. The Doc Tree View shows a framework and information about the framework on the right hand side, where logged in users with proper permissions can edit items, associate with other framework items, and copy other framework items into the current framework.

.. _h673d3c62a785f726a6b6333444e4b70:

2.2 OpenSALT Home Page
----------------------

The image below is an example of an OpenSALT site, OpenSALT.net hosted by PCG. When user launches opensalt.net in a browser, the user is presented with the open view of the site.

.. image:: static/OpenSALT_User_Manual_2.png
   :height: 102 px
   :width: 624 px


This is a view of an OpenSALT site hosted by ACT, located at frameworks.act.org

.. image:: static/OpenSALT_User_Manual_3.png
   :height: 104 px
   :width: 624 px


All public, non-provisioned users are able to view the frameworks and content with each form this view. Navigating the frameworks will be further discussed in a later section of this document.

.. _h6a553f521677b3b627ff294828321:

2.3 Log into OpenSALT
----------------------

For provisioned users the **Sign in** button will launch a login screen that will enable deeper system usage and open up available menus for further interaction with OpenSALT.

.. image:: static/OpenSALT_User_Manual_4.png
   :height: 204 px
   :width: 366 px


Provisioned users can enter in their *Username* (user’s email) and *Password* then click the **Login** button to access the admin functions for OpenSALT.

.. image:: static/OpenSALT_User_Manual_5.png
   :height: 116 px
   :width: 624 px


After logging in a provisioned user will now see the *Sign In* button replaced by “Signed in as *username*” (email) with a menu icon  and two new buttons on the main frame of the page:  **Create a new Framework** and **Import Framework**

.. _h5b52241c7178667e18023622a381f1:

2.4 Log off from OpenSALT
-------------------------

All provisioned users should log out of OpenSALT when finished with their session. To logout, click on the expansion menu next to the user name and select **Sign out**.

.. image:: static/OpenSALT_User_Manual_6.png
   :height: 150 px
   :width: 204 px


.. _h1b685a27e68c571dd1c317e122f34:

3.0  User Roles and Permissions
===============================

OpenSALT currently has five user roles with specified permissions for the tool:

#. Super User

#. Super Editor

#. Organization Administrator

#. Organization Editor

#. Organization Reviewer (Account in org but no role)

#. Public (non-authenticated)

The Chart below provides an overview of the users and their provisioned roles and detailed descriptions follow.

+-----------------+--------------+--------+-----------+--------------+-----------+
|User Type        |Logged in User|Editor  |Org Admin  |Super Editor  |Super User |
+=================+==============+========+===========+==============+===========+
|Access Frameworks|      X       |     X  |     X     |       X      |     X     |
+-----------------+--------------+--------+-----------+--------------+-----------+
|Edit a framework |              |        |           |              |           |
|in their own     |              |    X   |     X     |      X       |     X     |
|organization     |              |        |           |              |           |
+-----------------+--------------+--------+-----------+--------------+-----------+
|Edit a framework |              |   X    |     X     |    X         |    X      |
+-----------------+--------------+--------+-----------+--------------+-----------+
|Export frameworks|     x        |    x   |     X     |     X        |    X      |
+-----------------+--------------+--------+-----------+--------------+-----------+
|View Comments    |     x        |    x   |     X     |     X        |    X      |
+-----------------+--------------+--------+-----------+--------------+-----------+
| Manage Framework|              |        |           |              |           |
| rights          |              |        |     X     |     X        |    X      |
+-----------------+--------------+--------+-----------+--------------+-----------+
| Manage framework|              |        |           |              |           |
| ownership       |              |        |     X     |     X        |    X      |
+-----------------+--------------+--------+-----------+--------------+-----------+
| Edit Metadata   |              |        |           |      X       |    X      |
| across orgs     |              |        |           |              |           |
+-----------------+--------------+--------+-----------+--------------+-----------+
|Add/edit Users   |              |        |           |              |           |
|within an Org    |              |        |     X     |      X       |     X     |
+-----------------+--------------+--------+-----------+--------------+-----------+
|Add/Edit Orgs    |              |        |           |      X       |     X     |
+-----------------+--------------+--------+-----------+--------------+-----------+

Additionally, there are built in permissions regarding which users can edit organization-owned frameworks.

.. image:: static/user_orgs.png

.. _h155d6d5f4916497a1c6b10341f214165:

3.1 Super User
--------------

This is the top level in the user hierarchy for OpenSALT. A Super User has full permissions to the site and can create and manage organizations, manage users across all organizations, and manage all frameworks and content across all organizations.

* view any framework

* download (export) any framework in *Draft* or *Published* modes

* change their password

* add new, import, and edit frameworks in all organizations:

    * Personal frameworks

        * only editable by the creator (by default)

        * access can be granted to other editors to edit the framework

    * Organizational  frameworks

        * editable by all editors/admins in the organization (by default), this includes Super Editors and Super Admins

        * can edit frameworks which they have permission to edit:

            * frameworks owned by any organization

            * other frameworks where the user has been explicitly been granted edit access

        * alter edit access to any frameworks

        * assign ownership of any personal framework created by an editor in any organization

* manage organizations in OpenSALT

    * add organizations

    * edit organizations

    * delete organizations

* add users to any organization (Super User, Super Editor, Organization Admin or Organization Editor)

    * suspend users in any organization (Super User, Super Editor, Organization Admin or Organization Editor)

    * unsuspend users in any organization (Super User, Super Editor, Organization Admin or Organization Editor)

* Note the Super Users cannot be excluded from edit access to a framework

.. _h2b5616331387667a40761f394f7b10:

3.2 Super Editor
----------------

Much like the Super User, the Super Editor has has permissions to work across organizations however this user is only permitted to manage all frameworks and content across all organizations. The Super Editor has no access to manage organizations, nor users.

The Organization Admin can manage users for their given organization, and manage and manage all frameworks and content for only their organization.

* view any framework

* download (export) any framework in *Draft* or *Published* modes

* change their password

* add new, import, and edit frameworks in all organizations:

    * Personal frameworks

        * only editable by the creator (by default)

        * access can be granted to other editors to edit the framework

    * Organizational  frameworks

        * editable by all editors/admins in the organization (by default), this includes Super Editors and Super Admins

        * can edit frameworks which they have permission to edit:

            * frameworks owned by any organization

            * other frameworks where the user has been explicitly been granted edit access

        * alter edit access to any frameworks

        * assign ownership of any personal framework created by an editor in any organization

* Note the Super Editor cannot be excluded from edit access to a framework

.. _h4e2218295d122347968407129336e50:

3.3 Organization Admin
----------------------

The Organization Admin can manage users for their given organization, and manage and manage all frameworks and content for only their organization.

* view any framework

* download (export) any framework in *Draft* or *Published* modes

* change their password

* add new, import, and edit frameworks:

    * Personal frameworks

        * only editable by the creator (by default)

        * access can be granted to other editors to edit the framework

    * Organizational  frameworks

        * editable by all editors/admins in the organization (by default), this includes Super Editors and Super Admins

        * can edit frameworks which they have permission to edit:

            * frameworks owned by their organization open to all editors (no exclusions)

            * frameworks owned by their organization when the user is not in the exclusion list

            * other frameworks where the user has been explicitly been granted edit access

        * alter edit access to any frameworks owned by their organisation (personal frameworks)

        * assign ownership of any personal framework created by an editor in their organization

* add users to their organization (Organization Admin or Organization Editor)

    * suspend users in their organization (Organization Admin or Organization Editor)

    * unsuspend users in their organization (Organization Admin or Organization Editor)

.. _h223559828a7e63152e784375423e27:

3.4 Organization Editor
-----------------------

The Organization Editor has only access to its respective organization and is only permitted to manage frameworks and content with the assigned organization. An Organization Editor has no access to manage organizations, nor users. An Organization Editor can:

* view any framework

* download (export) any framework in *Draft* or *Published* modes

* change their password

* add new frameworks and import frameworks:

    * Personal frameworks

        * only editable by the creator (by default)

        * access can be granted to other editors to edit the framework

    * Organizational  frameworks

        * editable by all editors/admins in the organization (by default), this includes Super Editors and Super Admins

        * can edit frameworks which they have permission to edit:

            * frameworks owned by their organization open to all editors (no exclusions)

            * frameworks owned by their organization when the user is not in the exclusion list

            * other frameworks where the user has been explicitly been granted edit access

.. _h5ca4f6060522c494356773e1b9d6:

3.5 Organization Reviewer
-------------------------

The Organization Reviewer is an org member with no roles assigned. They can log in and access private draft frameworks in an organization. They can not edit or manage frameworks. An Organization Reviewer can:

* view any framework in an org, private or not

* download (export) any framework in *Draft* or *Published* modes

* change their password

* Add comments if comments are turned on

* They can **not** make personal frameworks.

.. _h6047727375e794d1cd6e73641d1357:

3.6 Public User
---------------

The Public User is the default user for all who visit an OpenSALT site. This user has no provisioned credentials and therefore cannot log into the site to access administrative functionality Rather this user is able to navigate the published frameworks and content and has read-only rights to the information. The Public User can:

* view any framework

* download (export) any framework in *Draft* or *Published* modes

.. _h6113256bc274e5e44d234a57614658:

4.0 Organization Management
===========================

**Audience: Super Users**

As discussed in section 2.1 Open SALT is designed to b a multi-tenant environment housing multiple organizations and users, though keeping all securely separated. In order to establish the separation, the Super User will need to create and manage organizations.

To access the **Manage Organization** page, after logging in the user should click the triangular menu icon next to their user name in the header of the page. The menu will expand with several options depending on the user’s role. Click on **Manage Organizations** to open the page.

.. image:: static/OpenSALT_User_Manual_8.png
   :height: 141 px
   :width: 188 px


The **Organization List**  is the default page displayed when a Super User accesses the **Manage Organization** function of OpenSALT. The list will display all organizations that the are currently in the given instance of OpenSALT. The **Organization List** provides the OpenSALT unique ID number, the Organization Name, and Actions for the organizations (**Show** and **Edit**). The page also has a button to **Add a new organization**.

.. image:: static/OpenSALT_User_Manual_9.png
   :height: 102 px
   :width: 624 px


.. _h2e38184e3252357f696d5953437a1433:

4.1 Show Organizations
----------------------

There are two ways to view an individual organization’s information beyond the **Organization list**  table view.

#. On the **Organization List** click on the linked **ID** number for the selected organization.

.. image:: static/OpenSALT_User_Manual_10.png
   :height: 81 px
   :width: 624 px


#. On the **Organization List** click on the **Show** button in the **Actions** section of the Organization table for the selected organization.

.. image:: static/OpenSALT_User_Manual_11.png
   :height: 82 px
   :width: 622 px


The **Organization** screen will display for the selected user.

.. image:: static/OpenSALT_User_Manual_12.png
   :height: 73 px
   :width: 624 px


The Super User can see the Organization’s unique ID value and the Organization’s name.

From the **Organization** screen the Super User can:

* return the **Organization List** by clicking the **Back to the list button**

* edit the organization by clicking on the **Edit** button

* delete the organization by clicking on the **Delete** button

.. _h3c64e441156177a1577f6b7b1f6b35:

4.2 Add/Create Organization
---------------------------

To create a new user, click on the **Add new user** button at the bottom right of the **User list**.

.. image:: static/OpenSALT_User_Manual_13.png
   :height: 29 px
   :width: 129 px


The Add an Organization page will display:

.. image:: static/OpenSALT_User_Manual_14.png
   :height: 57 px
   :width: 624 px


The admin will need to enter in the following required fields:

    *Name:* Type the Organization name

Then click on the **Add** button to create the organization.

If the Admin wants to cancel, and not create the organization, click the **Back to the list** button.

.. _h6e6b6c492a472a26603a601b4348370:

4.3 Edit Organization
---------------------

An Admin can access the **Organization edit** screen using two paths:

#. On the **Organization List** click on the **Edit** button in the **Actions** section of the Organization table for the selected organization.

.. image:: static/OpenSALT_User_Manual_15.png
   :height: 78 px
   :width: 622 px


#. On the **Organization** screen click on the **Edit** button.

.. image:: static/OpenSALT_User_Manual_16.png
   :height: 73 px
   :width: 624 px


The **Organization edit** screen will display and allow the Admin to update the user’s information.

.. image:: static/OpenSALT_User_Manual_17.png
   :height: 60 px
   :width: 624 px

The Admin can update/correct the following field:

    *Name:* Type the Organization name

Then click on the **Save** button to save the changes.

If the Admin wants to cancel, and not edit the the organization, click the **Back to the list** button.

The Admin can also delete the organization from this screen by clicking on the **Delete** button.

.. _h2e57757e4b2674d5e64291645c184:

4.4 Delete Organization
-----------------------

If an organization  needs to be completed removed from OpenSALT, the Admin should delete the organization. There are two methods to delete an organization.

#. From the **Organization List** click on the **Show** button for the selected organization. The **Organization** page will be displayed and the Admin can click the **Delete** button to terminate the organization. Once deleted the organization cannot be restored. If the organization is needed, the Admin will need to create a new organization.

.. image:: static/OpenSALT_User_Manual_18.png
   :height: 76 px
   :width: 624 px


#. From the **Organization List** click on the **Edit** button for the selected organization. The **Organization edit** page will be displayed and the Admin can click the **Delete** button to terminate the organization. Once deleted the organization cannot be restored. If the organization is needed, the Admin will need to create a new organization.

.. image:: static/OpenSALT_User_Manual_19.png
   :height: 60 px
   :width: 624 px


.. _h80265f116c6c7b4877762ed5412155:

5.0  User Management
====================

.. _h6d192e6d564f37133d53288be95d:

5.1 Change Password
-------------------

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

All provisioned users have the ability to change their password from the temporary one created by the Admin or as part of a good practice to regularly update their password to maintain a good security protocol.

To access the **Change Password** page, after logging in the user should click the triangular menu icon next to their user name in the header of the page. The menu will expand with several options depending on the user’s role. However all provisioned users will have the menu option: **Change Password**. Click on **Change Password** to open the page.

.. image:: static/OpenSALT_User_Manual_20.png
   :height: 129 px
   :width: 174 px


On the **Change Password** page the user will enter in the following required fields:

.. image:: static/OpenSALT_User_Manual_21.png
   :height: 116 px
   :width: 485 px

- **Old Password:** Existing current password

- **New Password:** Newly selected password

- **Repeat Password:** Re-type the newly selected password

- The user will then click the **Change Password** button.

If the entered values validate as correct, the old password is equal to the user’s current password and the new and repeat passwords are the same, the system will change the user's password to the newly selected value. If alny of the data is not validated, the system will prompt the user to correct the information before the change password can be completed.

.. _h42723a63d41151f712948537a568079:

5.2 Manage Users
----------------

**Audience: Super Users and Organization Admins**

User account management is controlled by the Super Users and the Organization Admins. To access the **Manage Users** page, after logging in the user should click the triangular menu icon next to their user name in the header of the page. Click on **Manage Users** to open the page.

.. image:: static/OpenSALT_User_Manual_22.png
   :height: 157 px
   :width: 210 px


.. _hfc27428297e2b766e5a37643a705f:

5.2.1 View User
~~~~~~~~~~~~~~~

**Audience: Super Users and Organization Admins**

The **User List** is the default page displayed when a Super User or Organization Admin accesses the **Manage User** function of OpenSALT. The list will display all users that the are currently in the given instance of OpenSALT. Super Users will see all users in all organizations, whereas Organization Admins will only see the users within their organization.  The User List will display the OpenSALT unique ID for the user (as system generated incremented number), the Organization the user belongs to, the Username (email) The user's role, and available actions (**show**, **edit**, **Suspend**) for the user. The page also has a button to **Add a new user**.

.. image:: static/OpenSALT_User_Manual_23.png
   :height: 150 px
   :width: 624 px


.. _h146b5979664d766a2a69263e3512862:

5.2.2 Add/Create User
~~~~~~~~~~~~~~~~~~~~~

**Audience: Super Users and Organization Admins**

To create a new user, click on the **Add new user** button at the bottom right of the **User list**.

.. image:: static/OpenSALT_User_Manual_24.png
   :height: 36 px
   :width: 105 px


The **Add a User** page will display:

.. image:: static/OpenSALT_User_Manual_25.png
   :height: 154 px
   :width: 624 px


The admin will need to enter in the following required fields:

    *Username*: Type the user’s email address

    Password: Type in a temporary password for the user. This password will not be viewable after creating the user. The Admin needs to take note of the temporary password entered to share with the user and the user will need to enter this password to change their password to a non-temporary secure password.

    *Role*: Select one role for the user and check the box accordingly

    *Org*: Select the user’s organization (note Organization Admins will only have their organization displayed, whereas Super Users will see all Organizations within the given OpenSALT site)

Then click on the **Add** button to create the user.

If the Admin wants to cancel, and not create the user, click the **Back to the list** button.

.. _h6e39602150137e754564a16671b646:

5.2.3 Show User
~~~~~~~~~~~~~~~

**Audience: Super Users and Organization Admins**

There are two ways to view an individual user’s information beyond the **User list** table view.

#. On the **User List** click on the linked **ID** number for the selected user.

.. image:: static/OpenSALT_User_Manual_26.png
   :height: 120 px
   :width: 584 px


#. On the **User List** click on the **Show** button in the **Actions** section of the User table for the selected user.

.. image:: static/OpenSALT_User_Manual_27.png
   :height: 128 px
   :width: 624 px


The **User** screen will display for the selected user.

.. image:: static/OpenSALT_User_Manual_28.png
   :height: 89 px
   :width: 624 px


The Super User or Organization Admin can see the user’s Organization, Username, and assigned Role.

From the **User** screen the Admin can:

*  return the **User List** by clicking the **Back to the list button**

* edit the user by clicking on the **Edit** button

* delete the user by clicking on the **Delete** button

.. _h6478147d1f4c85e5d62858217e145d:

5.2.4 Edit User
~~~~~~~~~~~~~~~

**Audience: Super Users and Organization Admins**

An Admin can access the **User edit** screen using two paths:

#. On the **User List** click on the **Edit** button in the **Actions** section of the User table for the selected user.

.. image:: static/OpenSALT_User_Manual_29.png
   :height: 150 px
   :width: 624 px


#. On the **User** screen click on the **Edit** button.

.. image:: static/OpenSALT_User_Manual_30.png
   :height: 88 px
   :width: 624 px


The **User edit** screen will display and allow the Admin to update the user’s information.

.. image:: static/OpenSALT_User_Manual_31.png
   :height: 154 px
   :width: 624 px

The Admin can update/correct the following fields:

    *Username*: If needed, type the user’s new email address. This will change the username that is entered when the user logs in.

    Password: If needed, type in a new temporary password for the user. This password will not be viewable after creating the user. The Admin needs to take note of the temporary password entered to share with the user and the user will need to enter this password to change their password to a non-temporary secure password.

    *Role*: If needed, select a new role for the user and uncheck the previous role.

    *Org*: If needed, change the organization Select the user’s organization (note Organization Admins will only have their organization displayed, whereas Super Users will see all Organizations within the given OpenSALT site)

Then click on the **Save** button to save the changes.

If the Admin wants to cancel, and not edit the the user, click the **Back to the list** button.

The Admin can also **delete** the user from this screen by clicking on the **Delete** button.

.. _h1cf396e28322d368416f6957481b1a:

5.2.5 Suspend User
~~~~~~~~~~~~~~~~~~

**Audience: Super Users and Organization Admins**

If an admin needs to prevent the user from accessing the OpenSALT instance, but needs to maintain the user’s account  in the system ,the admin can **Suspend** the user’s account.

To suspend an account the Admin will need to be on the User List page and select the **Suspend** button for the selected user.

.. image:: static/OpenSALT_User_Manual_32.png
   :height: 154 px
   :width: 624 px


After clicking on the **Suspend** button, the user will be immediately suspended. The **User list** is updated to reflect the suspension and the account can now only be viewed through the **Show** button or unsuspended with the **Unsuspend** button.

.. image:: static/OpenSALT_User_Manual_33.png
   :height: 24 px
   :width: 624 px


.. _h4d2e44565174e175b786376651a7d7c:

5.2.6 Reinstate User
~~~~~~~~~~~~~~~~~~~~

**Audience: Super Users and Organization Admins**

To reinstate a user’s account the Admin will access the **User List** and click on the **Unsuspend** button for the selected user. The **User list** will update and the account will be immediately unsuspended and the user can log in with the original credentials. If the user needs to have their password reset, the Admin can the edit the user by clicking the **Edit** button for the selected user and updated the password.

.. image:: static/OpenSALT_User_Manual_33.png
   :height: 24 px
   :width: 624 px


.. _h3c3329734240281c30b512222591212:

5.2.7 Delete User
~~~~~~~~~~~~~~~~~

**Audience: Super Users and Organization Admins**

If a user needs to be completed removed from OpenSALT, the Admin should delete the user. There are two methods to delete a user.

#. From the **User List** click on the **Show** button for the selected user. The **User** page will be displayed and the Admin can click the **Delete** button to terminate the user account. Once deleted the account cannot be restored. If the account is needed, the Admin will need to create a new user account.

.. image:: static/OpenSALT_User_Manual_34.png
   :height: 86 px
   :width: 624 px


#. From the **User List** click on the **Edit** button for the selected user. The **User edit** page will be displayed and the Admin can click the **Delete** button to terminate the user account. Once deleted the account cannot be restored. If the account is needed, the Admin will need to create a new user account.

.. image:: static/OpenSALT_User_Manual_31.png
   :height: 154 px
   :width: 624 px


.. _h26624554674c365425514b624a121c24:

6.0  Framework Management
=========================

.. _h1c4d1853674733a7f15411e4b788:

6.1 Navigate and View Frameworks
--------------------------------

OpenSALT is designed to be a simple application with few UI screens. The Application has two (2) primary screens for users to view and manage Frameworks and items:

#.  OpenSalt Home / Contents View Page

#. Framework Display Page

.. _h35526e50752d323810506420224185f:

6.1.1 OpenSalt Home / Contents View Page
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. _h1a7c6c1a163f6979313e611a1465218:

6.1.1.1 Public View
^^^^^^^^^^^^^^^^^^^

When a  user launches an OpenSALT instance through their browser they will reach the Public view of the OpenSALT site. The following images represent a few of the current OpenSALT sites in operation.

.. image:: static/OpenSALT_User_Manual_35.png
   :height: 266 px
   :width: 557 px


.. image:: static/OpenSALT_User_Manual_36.png
   :height: 268 px
   :width: 560 px


.. image:: static/OpenSALT_User_Manual_37.png
   :height: 265 px
   :width: 557 px


.. image:: static/OpenSALT_User_Manual_38.png
   :height: 265 px
   :width: 558 px


Note the default view has consistency from site to site. The variation is in the organization’s ability to add their organization logo and the content of the frameworks in the list.

Public users can view all Organizations with Draft and Adopted Frameworks on the OpenSALT site.

The default view is for all of the Organizations to be listed and their frameworks to be collapsed.

.. image:: static/OpenSALT_User_Manual_39.jpeg
   :height: 173 px
   :width: 565 px


The user can expand the Organizations to see all available Frameworks by clicking on either the arrow to the left of the Organization name or on the name itself.

.. image:: static/OpenSALT_User_Manual_40.jpeg
   :height: 217 px
   :width: 573 px


.. _h7997a7f1949334b7f84a24785861b:

6.1.1.2 Credentialed View
^^^^^^^^^^^^^^^^^^^^^^^^^

If a user has credentials and logs into OpenSALT they will have additional buttons on this page, depending on their role and permissions. Additionally they will be able to see all frameworks that are in a Private Draft status as well.

.. image:: static/OpenSALT_User_Manual_41.jpeg
   :height: 468 px
   :width: 446 px


.. _h715a2b6d63b2a41b18341215f345f:

6.1.2 Display Frameworks Page
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

When a user click on a framework on the **OpenSalt Home / Contents View Page** OpenSALT will open the **Framework Display** page for the select framework.

.. _h473664e5a545502f3e27165c142d:

6.1.2.1 Public View
^^^^^^^^^^^^^^^^^^^

.. image:: static/OpenSALT_User_Manual_42.jpeg
   :height: 357 px
   :width: 678 px


As a user clicks on a framework item, the Item Details frame will update to reflect the specifics for the selected item.

.. image:: static/OpenSALT_User_Manual_43.png
   :height: 505 px
   :width: 533 px


.. _hb622c455c38115d3972105a6f2f751e:

6.1.2.2 Credentialed View
^^^^^^^^^^^^^^^^^^^^^^^^^

Credentialed users will have additional administrative controls and functions on the Display Framework page, depending on their role and permissions.

.. image:: static/OpenSALT_User_Manual_44.jpeg
   :height: 285 px
   :width: 662 px

.. _hb622c455c38115d3972105a6f2f751f:

6.1.2.3 Log View
^^^^^^^^^^^^^^^^

Logged in Editors will have additional insights into what changes have been made on a framework by selecting the Log View Tab.

.. image:: static/log_loggedin.png

This view provides a comprehensive history of changes made to the framework in general as well as a method of exporting as a CSV file.

.. image:: static/log_full.png

.. _h473664e5a545502f3e27165c142e:

6.1.3 Adoption Status Security Features
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+-----------------+--------------+--------------+--------------+--------------+
|Draft Status     |Private Draft |Draft         |Adopted       |Deprecated    |
+=================+==============+==============+==============+==============+
|Public Can View  |Only with     |       No     |       No     |       No     |
|                 |specific link |              |              |              |
+-----------------+--------------+--------------+--------------+--------------+
|Org User can edit|      No      |       No     |       No     |       No     |
+-----------------+--------------+--------------+--------------+--------------+
| Non-Org editor  |Must be shared|Must be shared|Must be shared|Must be shared|
|    can edit     |              |              |              |              |
+-----------------+--------------+--------------+--------------+--------------+
|Access Frameworks|      X       |     X        |     X        |       X      |
+-----------------+--------------+--------------+--------------+--------------+

.. _h6e1cc76c3a603b3c6b78172573b9:

6.2 OpenSALT Frameworks
-----------------------

.. _h13a3f4f5767166b3c411a397a2511b:

6.2.1 Import Frameworks
~~~~~~~~~~~~~~~~~~~~~~~

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

OpenSALT has two methods for importing in an existing CASE-compliant framework into the site.

1) Import a CASE Compliant (JSON) file
2) Import a non-CASE compliant Spreadsheet file

.. _h3f23193f6633791f3f387f632bb3d54:

6.2.1.1 Import CASE-Compliant (JSON) File
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

OpenSALT allows users to import known CASE-compliant framework files into the system. Click on the **Import CASE file** tab in the  **Import Framework** window. Then click **Choose File.**

.. image:: static/OpenSALT_User_Manual_56.png
   :height: 180 px
   :width: 521 px


Navigate on your computer to the correct Case-compliant JSON file to import then  click **Open**.

.. image:: static/OpenSALT_User_Manual_57.png
   :height: 268 px
   :width: 530 px


The filename will display in the Choose File box, then click the **Import Framework** button to import the framework.

.. image:: static/OpenSALT_User_Manual_58.png
   :height: 171 px
   :width: 489 px


To cancel the action and not import the file, click on the **Close** button.

.. _h3f23193f6633791f3f387f632bb3d55:

6.2.1.2 Import Framework from spreadsheet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: static/OpenSALT_User_Manual_spreadsheet.png
   :height: 171 px
   :width: 489 px

On the Import screen, you are able to import a spreadsheet. For the spreadsheet importer, FullStatement is again the primary required field.
Screenshot of a sample file (template and larger sample located here_:

.. _here: https://github.com/opensalt/opensalt/tree/develop/sample%20files

.. image:: static/spreadsheet_sample.png

If the framework you are importing already exists on the server, it will update that framework and let you know with a message.

.. _h1d5d104a7b4f6a7c4a7715d503b1470:

6.2.2  Manually Create Frameworks
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

To Create a **Framework** manually the credentialed user will click on the Create a new Framework button on the **Framework Contents/OpenSalt Homepage** after logging into OpenSALT.

.. image:: static/OpenSALT_User_Manual_59.png
   :height: 121 px
   :width: 234 px


On the **Framework Creation** page, completed at a minimum the mandatory fields, though all fields should be filled in by best practice.

.. image:: static/OpenSALT_User_Manual_60.png
   :height: 358 px
   :width: 624 px


The following fields will display on the **LsDOC Creation** page:

* *Title:* The title as it appears on the cover of the Official Source artifact, although it may be a title created by the Publisher. This is a mandatory field in OpenSALT. .

* *Creator:* The the entity that authorized or created the competency framework. It could be an education agency, higher education institution, professional body. It is the owner of the competency framework (e.g CCSSO, TEA, NGSS). This is a mandatory field for OpenSALT and will act as the Organization Folder on the Framework Contents/OpenSALT Home page.

* *Official URI:* The URL of the artifact adopted by the Standard Setting Entity. Often this document is published in html and/or as pdf and is used by the standard setting entity as part of its approval process. Since it is not the intent of this specification to fully reproduce the human-facing content and formatting of the source document, it is recommended that this document be transmitted as part of the competency framework package. This is an optional field in OpenSALT, though best practices indicate it should be filled in.

* *Publisher:* The entity that loads and publishes the Framework. Note that in  many cases, the Standard Setting Entity may lack technical capabilities to publish the Competency Framework in a standard format so a third party may be displayed. This is an optional field in OpenSALT, though best practices indicate it should be filled in.

* *URL Name:* This field allows users to enter in a user friendly URL name. example: \ |LINK6|\  vs  \ |LINK7|\

.. |LINK6| raw:: html

    <a href="https://salt-staging.edplancms.com/cftree/doc/CSSS" target="_blank">https://salt-staging.edplancms.com/cftree/doc/CSSS</a>

.. |LINK7| raw:: html

    <a href="https://salt-staging.edplancms.com/cftree/doc/45" target="_blank">https://salt-staging.edplancms.com/cftree/doc/45</a>


* *Owned By:* Users will have the option to select from a few choices to indicate the Organization that created the Framework in OpenSALT.

    * *Me* - Private Framework created by an individual user

    * *My Organization* - Default to the user’s organization

    * *Other Organization (Named in the Dropdown)* - Super Editor or Super User can select any Organization in OpenSALT.

* *Version:* This is used to separate any version information expressed by the Official Source artifact. Once and CF Pkg has been approved and published, any changes to an CF Item will constitute a new version of the CF Doc. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Description:* The description is typically created by the the Publisher as a standard description of the Competency Framework.This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Subjects:* This is a string expressing the general subject area of the Competency Framework (e.g. Mathematics). This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Language:* HTML Language Country Code VIA- country code from \ |LINK8|\ . This is an optional field in OpenSALT, though best practice indicates the filled should be filled in. However OpenSALT assumes English if not other language value is entered.

.. |LINK8| raw:: html

    <a href="https://tooCF.ietf.org/html/bcp47" target="_blank">https://tooCF.ietf.org/html/bcp47</a>

* *Adoption Status:* Adoption status displays the Framework's current status as Draft, Private Draft,  Adopted, or Deprecated.  OpenSALT assumes Adopted as the default if no status is specifically selected for the framework. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank. OpenSALT assumes Adopted as the default if no status is specifically selected for the framework.

    * *Draft*: Able to be edited by Editors and Admins in an organization. Able to be viewed by the public.

    * *Private Draft*: Able to be viewed and edited by Editors and Admin in the owning organization

    * *Adopted*: Not able to be edited by Editors or Admin

    * *Depreciated:* Was once published, however it is now out of date

* *Status Start Date:* The date that the CF Doc status started. This is an optional field in OpenSALT.

* *Status End Date:* This date is often only known when a new status is started. This is an optional field in OpenSALT.

* *Note:* Notes or comments generated by the Framework Publisher about the context of the Framework. This is an optional field in OpenSALT.

To **create** the Framework, click the **Create** button.

To **cancel** and abandon any changes, click the **Back to the list** button.

When a Framework is created the **Framework Display** page will refresh and will indicate that are loaded with the framework.

.. image:: static/OpenSALT_User_Manual_61.png
   :height: 392 px
   :width: 624 px


Open SALT Provides the user with suggestions for how to add items to the framework.

.. image:: static/OpenSALT_User_Manual_62.png
   :height: 105 px
   :width: 624 px


.. _h2a278644e81e7672704d5078541c5:

6.2.3 Edit Frameworks
~~~~~~~~~~~~~~~~~~~~~

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

To **Edit** a **Framework** the credentialed user will select the appropriate **Framework** from the **Framework Contents/OpenSalt Home** Page by expanding the **Organization** and clicking on the desired **Framework**.


.. image:: static/OpenSALT_User_Manual_52.png
   :height: 216 px
   :width: 501 px


On the **Framework Display** page, click on the **Edit** button in the **Detail Frame**.

.. image:: static/OpenSALT_User_Manual_53.png
   :height: 185 px
   :width: 624 px


The **Edit Document** window will open and allow the user to update the necessary fields.

.. image:: static/OpenSALT_User_Manual_63.png
   :height: 522 px
   :width: 513 px


The following fields will display on the Edit Document window. Note some may be edited and others have fixed values:

* *Title:* The title as it appears on the cover of the Official Source artifact, although it may be a title created by the Publisher. This is a mandatory field in OpenSALT.

* *Creator:* The the entity that authorized or created the competency framework. It could be an education agency, higher education institution, professional body. It is the owner of the competency framework (e.g CCSSO, TEA, NGSS). This is a mandatory field for OpenSALT and will act as the Organization Folder on the Framework Contents/OpenSALT Home page.

* *Official URI:* The URL of the artifact adopted by the Standard Setting Entity. Often this document is published in html and/or as pdf and is used by the standard setting entity as part of its approval process. Since it is not the intent of this specification to fully reproduce the human-facing content and formatting of the source document, it is recommended that this document be transmitted as part of the competency framework package. This is an optional field in OpenSALT, though best practices indicate it should be filled in.

* *Publisher:* The entity that loads and publishes the Framework. Note that in  many cases, the Standard Setting Entity may lack technical capabilities to publish the Competency Framework in a standard format so a third party may be displayed. This is an optional field in OpenSALT, though best practices indicate it should be filled in.

* *URL Name:* This field allows users to enter in a user friendly URL name. example: \ |LINK9|\  vs  \ |LINK10|\

.. |LINK9| raw:: html

    <a href="https://salt-staging.edplancms.com/cftree/doc/CSSS" target="_blank">https://salt-staging.edplancms.com/cftree/doc/CSSS</a>

.. |LINK10| raw:: html

    <a href="https://salt-staging.edplancms.com/cftree/doc/45" target="_blank">https://salt-staging.edplancms.com/cftree/doc/45</a>

* *Owning Organization:* If a Framework is not a personal Framework, and rather is an Organizational Framework, the associated Organization that created or imported the Framework will be displayed. *Owning User:* If the Framework is a personal Framework owned by an individual user, the user’s name will be displayed. Otherwise the OpenSALT will assume a value of none because the Framework is not owned by a single user rather is owned by an Organization.

* *Version:* This is used to separate any version information expressed by the Official Source artifact. Once and CF Pkg has been approved and published, any changes to an CF Item will constitute a new version of the CF Doc. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Description:* The description is typically created by the the Publisher as a standard description of the Competency Framework.This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Subjects:* This is a string expressing the general subject area of the Competency Framework (e.g. Mathematics). This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Language:* HTML Language Country Code VIA- country code from \ |LINK11|\ . This is an optional field in OpenSALT, though best practice indicates the filled should be filled in. However OpenSALT assumes English if not other language value is entered.

.. |LINK11| raw:: html

    <a href="https://tooCF.ietf.org/html/bcp47" target="_blank">https://tooCF.ietf.org/html/bcp47</a>

* *Adoption Status:* Adoption status displays the Framework's current status as Draft, Private Draft,  Adopted, or Deprecated.  OpenSALT assumes Adopted as the default if no status is specifically selected for the framework. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank. OpenSALT assumes Adopted as the default if no status is specifically selected for the framework.

    * *Draft*: Able to be edited by Editors and Admins in an organization. Able to be viewed by the public.

    * *Private Draft*: Able to be viewed and edited by Editors and Admin in the owning organization

    * *Adopted*: Not able to be edited by Editors or Admin

    * *Depreciated:* Was once published, however it is now out of date

* *Status Start Date:* The date that the CF Doc status started. This is an optional field in OpenSALT.

* *Status End Date:* This date is often only known when a new status is started. This is an optional field in OpenSALT.

* *Note:* Notes or comments generated by the Framework Publisher about the context of the Framework. This is an optional field in OpenSALT.

To **save** the updated, click the **Save Changes** button.

To **cancel** and abandon any changes, click the **Cancel** button.

.. _ha6bf1778138296b7384e6b3d144c:

6.2.4 Delete Frameworks
~~~~~~~~~~~~~~~~~~~~~~~~~

**Audience: Super Users, Organization Admins**

OpenSALT allows Super Users and Organization Admins to delete Frameworks if needed. Note once a Framework is deleted the action can not be undone. The framework and all associations will be permanently removed from the database.

To delete a framework the Super User or Organization Admin will first need to log into OpenSALT.

Next view the selected Framework by expanding the organization and clicking on the selected Framework.

.. image:: static/OpenSALT_User_Manual_64.png
   :height: 224 px
   :width: 500 px



Once you are sure the correct Framework is selected and you are ready to **delete**, click the **Delete** button.

.. image:: static/OpenSALT_User_Manual_67.png
   :height: 500 px
   :width: 329 px


.. _h10414a76521969321d1aa7b43555d12:

6.2.5 Update Frameworks from a spreadsheet
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

OpenSALT allows organization admins and above to download a framework as an excel document and make the following changes that can be merged back into the framework on the server:
- Update an item's text based on the same guid (will overwrite any other field in that line)
- Add an item to the the spreadsheet - do not enter an identifier; one will be created for you on update
- Delete an item when removing the identifier

Other notes:
- If a parent statement is deleted, those children statements will be ungrouped as "orphans"

Note that the framework should only be updated from within the Document itself using the Update button. Furthermore, note that currently these changes are irreversible within the application. The Update code searches for the Cf Item identifier and then performs the update procedures described above based on that business logic. (Eg if it finds a new identifier, it adds the CF Item. If it does not find an identifier previously present, that item is removed from the server).

How-To `Video
<https://www.youtube.com/watch?v=thJb43wD6ZM&t=1s>`_

.. _h405471134e472ab58320531a7c433:

6.2.6 Create new associations via Spreadsheet Update Features
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

OpenSALT is able to use this function as well to update/create associations with generally the same user actions. Note that you have to be using the 'latest' spreadsheet download each time you update a framework.

.. _h405471134e472ab58320531a7c444:

6.2.6.1 Update Associations for frameworks on the same server

Simply enter the guids and association type you want in the appropriate columns on the Cf Association Tab of the downloaded spreadsheet. Do not enter an identiifer for the association action itself; this will be created by OpenSALT on upload.

.. image:: static/associations_update.png
   :height: 224 px
   :width: 500 px

.. _h405471134e472ab58320531a7c455:

6.2.6.2 Update Associations from an external server

This process is the same as for frameworks on the same server with two steps prior to the download, change, and update.

Steps:
1) Load an external framework within the framework you are working in.
2) Make one association from that document to the framework you are working on now.
3) Now use the guids from the external framework in the spreadsheet update tool as detailed above and the associations will load with connections to that external framework.

.. _h405471134e472ab58320531a7c456:

6.2.7  Copy Framework Only

When viewing a framework in the tree view, on the CF Document item detail pane you with sufficient rights you will see a button to Copy Framework. This will open up an additional dialog box for multiple options to copy the entire framework documents

.. image:: static/copyframeworkbutton.png

.. _h405471134e472ab58320531a7c457:

6.2.7.1 Copy Content Only

If you are intending on creating a new framework from the existing one, or simply with to add the current items to an existing framework, use this option. It will copy the framework items and structure and create new GUIDS for the items in the new framework. Associations are not transferred or created.

.. image:: static/copy_content.png

.. _h405471134e472ab58320531a7c458:

6.2.7.2 Copy and Make Derivative Framework

This will copy the framework items into a the target document and create Exact Match Of associations between origin and target items. No other associations will be copied. **There is a bug in OpenSALT 2.2 where a hard refresh is necessary before the copied CFItems are viewable to the user undertaking the copy action.**

.. image:: static/copy_derivative.png

.. _h10414a76521969321d1aa7b43555d10:

6.3 Framework Items
-------------------

Items can be created for Frameworks either by importing existing data using the OpenSALT template or by manually creating the items.

.. _h405471134e472ab58320531a7c422:

6.3.1 Import Items with OpenSALT Template
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Users can create their own CASE-compliant data files to load into OpenSALT using a provided template and guide. This allows users to easily import their items or standards into their created framework and eliminates the need for manually entering the data into the system. The template can be found here:  \ |LINK12|\ .

.. |LINK12| raw:: html

    <a href="https://docs.google.com/spreadsheets/d/1idJv2lHCU4xojCSm5vh_zBFhgUGQvvaNSwmdSzD3QIc/edit#gid=1492955133" target="_blank">Spreadsheet Loading Guide for CASE</a>

.. _h5777746416576973633711c4a42414c:

6.3.1.1 CSV Loading Guide for CASE
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

General notes when loading/creating CSV files for bulk upload of child statements:

The only required field to upload a framework is FullStatement, but to build a hierarchy you will need Human Coding Scheme as well as the two layers for IsChildOf.

If an identifier exists, it will be transferred to the OpenSALT system. If it does not exist one will be created upon upload and creation.

SequenceNumber may be used to denote a particular order within parent nodes.

Currently the only fields with Rich Text capability through markdown are FullStatement and Notes.

See "CASE.csv" in the /opensalt/sample files/.

Tab 1: Step 1 Read This

An Overview of the process for creating the CSV to import the data.

Step 1: Create New Framework

.. image:: static/OpenSALT_User_Manual_69.png
   :height: 49 px
   :width: 120 px


Step 2: Select “Import Children”

.. image:: static/OpenSALT_User_Manual_70.png
   :height: 89 px
   :width: 422 px


Step 3: Select your CSV

.. image:: static/OpenSALT_User_Manual_71.png
   :height: 152 px
   :width: 538 px


Step 4: If your CSV has associations to external frameworks in the full human readable terms (ie  CCSS.MATH.Content.K.CC.A.1) select the framework you want to associate it too. If nothing just leave alone

Step 5: Select Import Children

Tab 2: CF DOC

The only required fields are Creator and title. Creator is the folder that will be created.


Tab 3: CF ITEM

Explanation of the item fields that will be included in template for the Framework. Note that technically only fullStatement and humanCodingScheme are required.

The only required field is fullstatement.

To create a hierarchy however, use human coding scheme, ischildOf and SequenceNumber

example:

+---------------+------------------+-----------+----------------+
|fullStatement  |humanCodingScheme |IsChildOf  |SequenceNumber  |
+---------------+------------------+-----------+----------------+
|Parent Item    | P                |           | 1              |
+---------------+------------------+-----------+----------------+
|Child 1        | P.C              | P         | 1              |
+---------------+------------------+-----------+----------------+
| Grandchild 1  | P.C.G            | P.C       | 1              |
+---------------+------------------+-----------+----------------+
| Child 2       | P.C2             | P         | 2              |
+---------------+------------------+-----------+----------------+
| Grandchild 2  |P.C2.G            | P.C2      | 1              |
+---------------+------------------+-----------+----------------+


Tab 4: CF Association

The process for associations which can be associated in the template if desired, though associations may be easier managed in the UI itself after the Framework is created and imported.

.. image:: static/OpenSALT_User_Manual_74.png
   :height: 304 px
   :width: 682 px


Tab 6: Template

The template itself that will be used to add the data into the correct format and  saved as a CSV to import into OpenSALT.

You may use these fields as your template and save into a CSV.
+---------------+---------------+------------------+-----------+----------------+
|Identifier     |fullStatement | humanCodingscheme | IsChildOf | SequenceNumber |
+---------------+----------------+-----------+----------------+

.. _h9291733595a7a78664a32f6e6f6f12:

6.3.1.2 Import Process
^^^^^^^^^^^^^^^^^^^^^^

After reviewing the **CSV Loading Guide for CASE** and the user will need to format their data into the Template Tab then save the file locally to their computer as a CSV file. This will save only the Template Tab and convert the data from an Excel file to a CSV file for import.

.. image:: static/OpenSALT_User_Manual_77.png
   :height: 192 px
   :width: 624 px


Next the user will need to Import the items/children for the Frameworks. Click on the **Import Children** button in the **Item Details Frame** on the right of the selected framework to open the **Import Items** window.

.. image:: static/OpenSALT_User_Manual_78.png
   :height: 344 px
   :width: 566 px


Select the tab for where your template file is located. If the CSV is stored locally on your computer,  click on the Import local File tab. Browse and select your file with the Choose File button. If a specific Framework to be associated is preferred, mark that selection otherwise the default is All. Then click the Import Children button to import the items for the framework.

.. image:: static/OpenSALT_User_Manual_79.png
   :height: 220 px
   :width: 601 px


Alternatively if the template is stored in your GitHub repository, click on the Import from GitHUb tab and login to connect to your file and import the items for the framework.

.. image:: static/OpenSALT_User_Manual_80.png
   :height: 265 px
   :width: 588 px


The items will be loaded and the Framework Display page will be refreshed.

.. image:: static/OpenSALT_User_Manual_81.png
   :height: 304 px
   :width: 609 px




.. _h23320351bb10619415c7276b33c:

6.3.1.3  Error Log
^^^^^^^^^^^^^^^^^^

On import, error messages will display when a file is missing fields. These error messages can be retrieved afterwards by clicking on “error log” in the admin console.

.. image:: static/OpenSALT_User_Manual_82.png
   :height: 156 px
   :width: 460 px


(Sample log)

.. image:: static/OpenSALT_User_Manual_83.png
   :height: 172 px
   :width: 624 px


.. _h760426c237f1dae3397155354c:

6.3.2 Formatting for Full Statement
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Item full statements can be formatted using three different methods / pure UTF8 text can be enhanced with:

* Markdown

* LaTeX

* Limited HTML tags

These three formatting options for text can be combined in-line with limitations.

.. _h7d786e1625325662166b2742346719:

6.3.2.1 Using HTML Tags
^^^^^^^^^^^^^^^^^^^^^^^

As of OpenSALT build 1.3. Some HTML tags are allowed despite HTML sanitization. The tags that will render are:

ul, ol, li, b, i, u, br, p

.. _h492e1366cf237f7436427a47773430:

6.3.2.2 Using Markdown
^^^^^^^^^^^^^^^^^^^^^^

Note that since OpenSALT uses markdown(\ |LINK13|\ ) as the primary formatting language, there could be unintended formatting consequences when importing from external sources.

.. |LINK13| raw:: html

    <a href="https://github.com/markdown-it/markdown-it/tree/master/docs" target="_blank">markdown-it</a>

.. _h712252444f3010471e714d613052609:

6.3.2.3 Using LaTeX
^^^^^^^^^^^^^^^^^^^

The LaTeX system supports plain text writing of all KaTeX functions listed \ |LINK14|\ . In-line LaTeX is formatted as braced between dollar signs ($):

.. |LINK14| raw:: html

    <a href="https://khan.github.io/KaTeX/function-support.html" target="_blank">here</a>

.. image:: static/OpenSALT_User_Manual_84.png
   :height: 40 px
   :width: 624 px


Alternatively, block text LaTeX is formatted as braced between double dollar signs ($$).

(no screenshot available)

.. _h3c5d33407b22107e304457e6932141b:

6.3.2.4 Combining text and LaTeX in-line
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

LaTeX formatting may be combined in-line with plain text in the markdown editor:

.. image:: static/OpenSALT_User_Manual_85.png
   :height: 93 px
   :width: 624 px


.. _h4e5c635d39551b1721751d107e72a28:

6.3.2.5 Constraints for using HTML tags
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

HTML and LaTeX cannot be combined in-line with anything else.

.. _h5e7e11124273126f13a587e68482f6e:

6.3.2.6 Using the Modes of Markdown Editor UI
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The markdown editor is accessed by clicking on the “Edit” button for an item:

.. image:: static/OpenSALT_User_Manual_86.png
   :height: 302 px
   :width: 358 px


The markdown editor has 11 functional buttons to manipulate Full Statement text, from left to right they are: Bold, Italics, Heading, Quote, Generic List, Numbered List, Insert Table, Insert Horizontal Line, Toggle Preview, Toggle Side by Side, Toggle Full Screen. These text-editing options are depicted below:

.. image:: static/OpenSALT_User_Manual_87.png
   :height: 62 px
   :width: 434 px


In the subsections below example text is showin in two columns; the first column shows the Markdown special characters, while the right column shows the text in the way it presents to the end user.

Bold 6.3.2.6.1

Text may be **bolded** by clicking icon 1/11 in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_88.png
   :height: 29 px
   :width: 29 px


In the Markdown editor, Bold special character text is indicated by \*\* on either end of the statement:

.. image:: static/OpenSALT_User_Manual_89.png
   :height: 18 px
   :width: 624 px


Italics 6.3.2.6.2

Text may be *italicized* by clicking icon 2/11 in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_90.png
   :height: 30 px
   :width: 30 px


In the Markdown editor, Italics special character text is indicated by \* on either end of the statement:

.. image:: static/OpenSALT_User_Manual_91.png
   :height: 26 px
   :width: 624 px


Heading 6.3.2.6.3

Text may be converted into a header by clicking icon 3/11 icon in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_92.png
   :height: 28 px
   :width: 32 px


In the Markdown editor, Heading special character text is indicated by #, which precedes the statement:

.. image:: static/OpenSALT_User_Manual_93.png
   :height: 57 px
   :width: 624 px


Quote 6.3.2.6.4

Text may be converted into a header by clicking icon 4/11 icon in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_94.png
   :height: 28 px
   :width: 30 px


In the Markdown editor, Quote special character text is indicated by >, which precedes the statement:

.. image:: static/OpenSALT_User_Manual_95.png
   :height: 53 px
   :width: 624 px


Generic List 6.3.2.6.5

Text may be converted into a bulleted list by clicking icon 5/11 icon in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_96.png
   :height: 29 px
   :width: 34 px


In the Markdown editor, Generic List special character text is indicated by >, which precedes the statement:

.. image:: static/OpenSALT_User_Manual_97.png
   :height: 62 px
   :width: 624 px


Numbered List 6.3.2.6.6

Text may be converted into an enumerated list by clicking icon 6/11 icon in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_98.png
   :height: 34 px
   :width: 36 px


In the Markdown editor, Generic List special character text is indicated by \*, which precedes the statement:

.. image:: static/OpenSALT_User_Manual_99.png
   :height: 57 px
   :width: 624 px


Insert Table 6.3.2.6.7

A table may be inserted by clicking icon 7/11 icon in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_100.png
   :height: 28 px
   :width: 28 px


In the Markdown editor, Columns headings and associated text are separated by inserting a Horizontal Line:

.. image:: static/OpenSALT_User_Manual_101.png
   :height: 78 px
   :width: 624 px


Insert Horizontal Line 6.3.2.6.8

A horizontal line may be inserted by clicking icon 8/11 icon in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_102.png
   :height: 32 px
   :width: 29 px


In the Markdown editor, a solid horizontal line is indicated by ----- between text statements:

.. image:: static/OpenSALT_User_Manual_103.png
   :height: 122 px
   :width: 624 px


Toggle Preview 6.3.2.6.9

An editor toggle between Markdown special characters vs. end user  view of text by clicking icon 9/11 icon in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_104.png
   :height: 29 px
   :width: 30 px


The toggle shifts between preview mode and pure text edit mode.

Toggle SIde by Side 6.3.2.6.10

An editor may view Markdown pure text and its rendered view simultaneously by clicking icon 10/11 icon in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_105.png
   :height: 29 px
   :width: 30 px


This two column view is depicted in all examples above and is the easiest way to edit and format text.

Toggle Full Screen 6.3.2.6.11

An editor may expand the Full Statement textarea by clicking icon 11/11 icon in the Full Statement toolbar:

.. image:: static/OpenSALT_User_Manual_106.png
   :height: 29 px
   :width: 30 px


This does not cause the area to expand to the full monitor width, bur rather to the width of the pop-up dialogue.

Underline 6.3.2.6.12

Underline may be utilized by entering Markdown’s emphasis tag, or placing _underscore_ on either end of a word or phrase.

.. _h692547f3e2dc3667114b432974477:

6.3.2.7 Other Considerations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Line Break after markdown table requires the following input: $~$ or an HTML <br>

.. _h439621724a6868657a4a744a69c71:

6.3.3 Create Items Manually
~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

When a Framework is created it is item neutral and is open for organizational content to be added based on the user’s needs. In addition to the Item import in section \ |LINK15|\ , OpenSALT allows users to manually create items and organize the data through the OpenSALT UI.

.. |LINK15| raw:: html

    <a href="#heading=h.6jki613css7u">6.5.1</a>

On the **Framework Display** page, click on the Item or Framework name that will act as a parent for the item to be added. Then in the **Item Details Frame** click on the **Add New Child Item** button.

.. image:: static/OpenSALT_User_Manual_107.png
   :height: 185 px
   :width: 624 px


The **Add New Child Item** window will display.

Enter in the appropriate values for all available fields. At a minimum enter in  mandatory **Full Statement.**

* *FullStatement*: The the main content of the CF Item. It is used to express both nodes and granular statements. If the statement is part of a list, the list enumeration should not be included in the statement and should instead be contained in the List Enumeration in Source Document. This is a mandatory field in OpenSALT.

* *HumanCodingScheme*: The ID sometimes used by humans to identify a CF Item. It often will use concatenated codes expressing its position in the taxonomy and abbreviations to convey other classification information (e.g. K.CC.1.1). This is an optional field in OpenSALT.

* *ListEnumeration*: Used to parse out enumerations or bullets that precede CF Item statements. This is an optional field in OpenSALT..

* *AbbreviatedStatement:* Abbreviated or summary statement provided by the Publisher. This is an optional field in OpenSALT and may be blank.

* *ConceptKeywords:* Upper level CF Item node statements may be used to populate Concept Keywords of lower level nodes. upper The concepts data structure allows a master list of keywords to be defined which can then be parsed down specific to a node. This works as usually concepts will be a less granular hierarchy representation of of the more detailed nodes in CF items. A node could be 'Geometry' and the lower node is 'Tangents' but the keywords for 'tangents' could include the word geometry. This is an optional field in OpenSALT and may be blank.

* *Language:* HTML Language Country Code VIA- country code from \ |LINK16|\ . This is an optional field in OpenSALT. If best practices are not followed, this field may be blank. However OpenSALT assumes English if not other language value is entered.

.. |LINK16| raw:: html

    <a href="https://tooCF.ietf.org/html/bcp47" target="_blank">https://tooCF.ietf.org/html/bcp47</a>

* *EducationLevel:* 	The current US K12 defined vocabulary is to use CEDS https://ceds.ed.gov/cedselementdetaiCF.aspx?termid=8267. Multiple values are allowed via comma delimitation and should be used to express grade spans. This is an optional field in OpenSALT and may be blank.

* *ItemType:* e.g., "Standard," "Benchmark," "Strand," or "Topic." or "Level 1, Level 2,..." This is an optional field in OpenSALT and may be blank.

* *License uri:*  Systems may filter for content with particular licences to support discovery. This is an optional field in OpenSALT and may be blank.

* *Notes:* In some cases, this can be used to contain additional information found in the original source document. This is an optional field in OpenSALT and may be blank.

.. image:: static/OpenSALT_User_Manual_108.png
   :height: 430 px
   :width: 496 px


To **create** the item, click the **Create** button.

To **cancel** and discard the changes, click the **Cancel** button.

.. _h3e4c72359f11834c363160506a4f:

6.3.4 Parent vs Child Items
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Once the Item is created it will by default only be a child of the item it was created for.

.. image:: static/OpenSALT_User_Manual_109.png
   :height: 241 px
   :width: 590 px


To add items nested below the item created, the user will need to make this item a Parent item. Highlight the item on in the **Framework Display** and click on the **Make This Item a Parent** button in the **Item Detail Frame**.

.. image:: static/OpenSALT_User_Manual_110.png
   :height: 252 px
   :width: 617 px


The bullet icon on the left of the item in the **Framework Display** will update to reflect it is now a P**arent item**  and the buttons in the **Item Detail Frame** will update to allow the user to either downgrade back to a child with the **Make This Item a Child** button or to add a new child for this parent item with the **Add a New Child** *button.*

The user can toggle the item between **Parent or Child** as necessary by clicking the **Make This Item a Parent** or **Make this Item a Child** buttons respectively.

Note an item can be a Child of an item and a Parent to other items, however an item can not be a Child of an item with children below it. This item must be upgraded to a Parent to have children.

.. image:: static/OpenSALT_User_Manual_111.png
   :height: 254 px
   :width: 624 px


The user can repeat this process an unlimited number of times to continue adding all items and marking them as Parents when appropriate to complete the full content for the framework.

.. image:: static/OpenSALT_User_Manual_112.png
   :height: 296 px
   :width: 584 px


.. image:: static/OpenSALT_User_Manual_113.png
   :height: 382 px
   :width: 440 px


.. image:: static/OpenSALT_User_Manual_114.png
   :height: 285 px
   :width: 562 px


.. image:: static/OpenSALT_User_Manual_115.png
   :height: 301 px
   :width: 624 px


.. _h8201a81d2a91674762e145b5a4931:

6.3.5 Edit Items
~~~~~~~~~~~~~~~~

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

.. _h5e35241f59206069503f4201efa4e:

6.3.5.1 Edit Item Content
^^^^^^^^^^^^^^^^^^^^^^^^^

To **edit** an item, the user must click on the item in the **Framework Display** and then click on the **Edit** button in the **Item Detail Frame.**

.. image:: static/OpenSALT_User_Manual_116.png
   :height: 264 px
   :width: 581 px


The **Edit Item** window will display. And the user can alter the data fields as needed.

.. image:: static/OpenSALT_User_Manual_117.png
   :height: 361 px
   :width: 414 px


To **save** the changes, click the **Save Changes** button.

To **cancel** and discard the changes , click the **Cancel** button.

.. _h69157d55e5f605ba4d2a777f3b1e2b:

6.3.5.2 Edit Item Positions
^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

OpenSALT enables users to move items within frameworks and reorder without the need to edit each item. The user must first enable the functionality but checkin on the box at the top of the Framework Display to Enable drag-drop reordering.

.. image:: static/OpenSALT_User_Manual_118.png
   :height: 196 px
   :width: 456 px


With the box checked and the function enabled, the user can now click on an item and drag and drop it to another location. Note clicking on a child will only move the child, whereas selecting a Parent will move the parent and all of it’s children.

.. image:: static/OpenSALT_User_Manual_119.png
   :height: 233 px
   :width: 302 px
.. image:: static/OpenSALT_User_Manual_120.png
   :height: 233 px
   :width: 304 px


Note with the drag and drop feature, items can be indented (moved to new parents) outdented to become parents, and all data can be fully moved around. However once an item is moved, there is no undo button, so the user would need to manually move (drag/drop) the item to the original position if the move is not required or done in error. Because of this, the feature is always defaulted to unchecked so no errors are accidentally made.

.. _h74193831603277236269697960746e75:

6.3.6 Delete Items
~~~~~~~~~~~~~~~~~~

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

All credentialed users can delete items that they have access to edit.

.. _h496724721a584f59624426723f296750:

6.3.6.1 Delete Child Item
^^^^^^^^^^^^^^^^^^^^^^^^^

To **delete** a child item, the user must click on the item in the **Framework Display** and then click on the **Delete** button in the **Item Detail Frame.**

.. _h336e6a1d1678622c20691174730325d:

.. image:: static/OpenSALT_User_Manual_121.png
   :height: 261 px
   :width: 576 px

------------

The delete action can not be undone. The user will be prompted with a warning message and must acknowledge the action cannot be reversed by clicking on the **Delete** button to proceed.

.. image:: static/OpenSALT_User_Manual_122.png
   :height: 104 px
   :width: 508 px


To cancel and leave the item in the Framework, click the **Cancel** button.

.. _h49d7804e5e24335978136f7c3b385e:

6.3.6.2 Delete Parent Item
^^^^^^^^^^^^^^^^^^^^^^^^^^

To **delete** a parent item, the user must click on the item in the **Framework Display** and then click on the **Delete** button in the **Item Detail Frame.**

.. _h2137497f644f6de4c4c69506531722d:

.. image:: static/OpenSALT_User_Manual_123.png
   :height: 305 px
   :width: 586 px

------------

The delete action can not be undone. The user will be prompted with a warning message that the item and all of it’s children will be deleted if the user proceeds. The user and must acknowledge the action cannot be reversed by clicking on the **Delete** button to proceed.

.. image:: static/OpenSALT_User_Manual_124.png
   :height: 129 px
   :width: 564 px


To cancel and leave the item in the Framework, click the **Cancel** button.

.. _h417d2d687a6e463a4f2e12321e305c68:

6.4 Exemplars for Items
-----------------------

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

OpenSALT provides the ability for a user to connect an example or **Exemplar** to any item within a Framework.  Note the Exemplars can not be associated to the Framework, rather only the items within. However an Exemplar can be associated to a Parent or a Child Item.

.. _h1f2d7057546c742f477446913652e37:

6.4.1 Add Exemplar
~~~~~~~~~~~~~~~~~~

To connect an example or **Exemplar** to an item. Select the item within the framework on the **Framework Display** page. Then click on the **Add Exemplar** button on in the **Item Details Frame**.

.. image:: static/OpenSALT_User_Manual_125.png
   :height: 214 px
   :width: 602 px


The **Add an Exemplar** window will open.

.. image:: static/OpenSALT_User_Manual_126.png
   :height: 185 px
   :width: 604 px


The user can either enter in a URL to an Exemplar or type text into the box. To save the Exemplar, click on the **Add Exemplar** button. To discard changes click on the **Cancel** button.


After clicking the **Add Exemplar** button, the F**ramework Display** page will refresh and the exemplar is linked to the item. This can be verified in the **Item Detail Frame**.

.. image:: static/OpenSALT_User_Manual_127.png
   :height: 284 px
   :width: 624 px


.. _h121a4c79224b7fc925545a2e64286f:

6.4.2 Delete Exemplar
~~~~~~~~~~~~~~~~~~~~~

To delete an **Exemplar** from an item, click on the ‘**x**’ icon next to the exemplar detail in the **Exemplar section** of the I**tem Detail Frame** on the **Framework Display** page. Note this action can not be reversed once completed. The user will be promoted with a warning message to proceed.

.. image:: static/OpenSALT_User_Manual_128.png
   :height: 337 px
   :width: 449 px


Note this action can not be reversed once completed. The user will be promoted with a warning message and must acknowledge the **OK** button to proceed.

.. image:: static/OpenSALT_User_Manual_129.png
   :height: 124 px
   :width: 372 px

.. _h38345071571251147d64497174403132:

6.5 Derivative Frameworks - Copy Items
--------------------------------------

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

OpenSALT allows users to create derivative frameworks  from frameworks within an OpenSALT server or instance.  Creating a derivative framework allows organizations to take a base original copy of a framework and expand it to better meet its needs.  The illustration below shows how the derivative frameworks fit with the scope of frameworks as a whole. Derivative frameworks essentially act as a bridge for organizations to navigate education needs.

.. image:: static/OpenSALT_User_Manual_130.jpeg
   :height: 348 px
   :width: 553 px


The user will need to be logged into OpenSALT and create or select the framework that will act as the new derivative framework or copy. Please see section \ |LINK17|\  if assistance is needed on how to create a framework. On the **Framework Display** page, click on the **Copy Items** button in the **Item Detail** frame.

.. |LINK17| raw:: html

    <a href="#heading=h.uzlj2tpaic68">6.2.2  Manually Create Frameworks</a>

.. image:: static/OpenSALT_User_Manual_131.png
   :height: 168 px
   :width: 624 px


In the C**opy Items** frame select the document/Framework to copy. Note if the framework to copy is not listed in the document view it is not currently on the OpenSALT server. Please see section \ |LINK18|\  for instructions on importing frameworks into OpenSALT.

.. |LINK18| raw:: html

    <a href="#heading=h.e03op9mhzcs2">6.2.1</a>

Select the desired framework in the **Document** dropdown. The Copy ITems frame will refresh and load the selected framework so its items can be viewed.

.. image:: static/OpenSALT_User_Manual_132.png
   :height: 149 px
   :width: 624 px


The user can now select individual items or the full set to copy over to the derivative framework on **Framework Display** on the left.

To select and copy a single item, expand the framework to the level/item desired. Click on the item and drag and drop it to the appropriate location on the left.

.. image:: static/OpenSALT_User_Manual_133.png
   :height: 229 px
   :width: 624 px


.. image:: static/OpenSALT_User_Manual_134.png
   :height: 230 px
   :width: 624 px


When the user releases the item on the left, the framework will refresh and the item will now display as part of the framework.

.. image:: static/OpenSALT_User_Manual_135.png
   :height: 301 px
   :width: 573 px


A user can select a parent item and add it to the framework, which will copy over all children under the parent as well.

.. image:: static/OpenSALT_User_Manual_136.png
   :height: 250 px
   :width: 624 px


.. image:: static/OpenSALT_User_Manual_137.png
   :height: 201 px
   :width: 397 px


To select multiple items at once the user can expand the multi select function by clicking on the empty checkbox above the framework displayed in the Copy Items frame.

.. image:: static/OpenSALT_User_Manual_138.png
   :height: 145 px
   :width: 289 px


The user can now check one or more boxes and click on an item to drag and drop to the left. All items selected will move. Note if a Parent is selected all the children will also move with it even if they are not individually checked.

.. image:: static/OpenSALT_User_Manual_139.png
   :height: 290 px
   :width: 266 px


Note to close the multi select function, click on **Actions** and select **Hide Checkboxes**.

.. image:: static/OpenSALT_User_Manual_140.png
   :height: 186 px
   :width: 293 px


.. image:: static/OpenSALT_User_Manual_141.png
   :height: 272 px
   :width: 278 px


.. _h3130761b154e2b57715e7f2385a5548:

6.6 Association Management
--------------------------

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

OpenSALT provides users with a robust way to include associations following the IMS GLobal CASE Standards. The application enables users to connect frameworks and framework items together to bring together relationship models that integrate and blend frameworks in a meaningful way.  The illustration below provides a visual mapping for how associations can connect frameworks and help to crosswalk standards.

.. image:: static/OpenSALT_User_Manual_142.jpeg
   :height: 342 px
   :width: 492 px


.. _h7529305c281925361d6f9354e774716:

6.6.1 Associations
~~~~~~~~~~~~~~~~~~

OpenSALT allows for the associations defined by \ |LINK19|\ . The permitted associations are:

.. |LINK19| raw:: html

    <a href="https://www.imsglobal.org/sites/default/files/CASE/casev1p0/information_model/caseservicev1p0_infomodelv1p0.html#Enumerated_CFAssociationTypeEnum" target="_blank">IMS Global’s CASE specification as noted in figure 7.3.1</a>

|

    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
    |Association Type|Description                                                                                                                                                                                                                     |Commentary (Unofficial, not representative of official CASE documentation)        |
    +================+================================================================================================================================================================================================================================+==================================================================================+
    |exactMatchOf    |Equivalent to. Used to connect derived CFItem to CFItem in original source CFDocument.                                                                                                                                          |Used to connect derivative framework statements.                                  |
    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
    |exemplar        |The target/destination node is an example of best practice for the definition of the source/origin.                                                                                                                             |Point to a learning resource or other public artifacts(Unlimited).                |
    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
    |hasSkillLevel   |The destination of this association is understood to define a given skill level i.e. Reading Lexile 100, Depth Knowledge 2, or Cognitive Level (Blooms Taxonomy) etc.                                                           |Used to capture equivalencies between different types of frameworks.              |
    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
    |isChildOf       |To represent the structural relationship in a taxonomy between parent and child. The source/origin is a child of the target/destination.                                                                                        | Groups children statements with their parent statement.                          |
    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
    |isPartOf        |The origin of the association is included either physically or logically in the item at the destination of the association. This classifies an item as being logically or semantically contained as a subset of the destination.|As an example, if three skills of a framework are subsets of one skill in another.|
    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
    |isPeerOf        |The source/origin is a peer of of the target/destination.                                                                                                                                                                       |Equivalence across frameworks when no grade level is given.                       |
    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
    |isRelatedTo     |The origin of the association is related to the destination in some way that is not better described by another association type.                                                                                               |Use is acceptable for learning resources but not as specific as assessment results|
    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
    |precedes        |The origin of the association comes before the destination of the association in time or order.                                                                                                                                 |For creating learning maps/progressions.                                          |
    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+
    |replacedBy      |The origin of the association has been supplanted by, displaced by, or superseded by the destination of the association.                                                                                                        |For showing equivalence across versions.                                          |
    +----------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------+


.. _h5b382e5f3a7b484e5e49c7b706545f:

6.6.1.1 Create Associations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

OpenSALT allows users to create associations to and between Framework items that either reside in the same OpenSALT instance or to any other outside CASE-compliant system.

To create an association, open the Framework target in the **Framework Dispaly** page.then click **Create Associations** to open the Associations frame.

.. image:: static/OpenSALT_User_Manual_143.png
   :height: 237 px
   :width: 580 px


In the Document dropdown, select the framework you want to use with the associations.  If the framework is within the OpenSALT server instance, the framework name will display organized by the owning Organization.

.. image:: static/OpenSALT_User_Manual_144.png
   :height: 342 px
   :width: 624 px


Click on the required Framework to display the framework and items.

Alternatively you can select The final option: **Load an “external” document by url…** This allows the user to select any CASE compliant framework that is stored on an external location.

The **Load External Document** window will display. The user will need to copy and paste, or type in the url for the Case-compliant framework.

.. image:: static/OpenSALT_User_Manual_145.png
   :height: 186 px
   :width: 568 px


In instances of OpenSALT, the **Case Framework URL** can be found on the **Framework Display** page in the **Item Detail** frame.

.. image:: static/OpenSALT_User_Manual_146.png
   :height: 170 px
   :width: 624 px


Note if the copied URL does not have the .JSON extension, you will need to add it for the document to load.

.. image:: static/OpenSALT_User_Manual_147.png
   :height: 204 px
   :width: 624 px


To load the framework, click the **Load Document** button.

To cancel and return to the **Framework Display** page, click the **Cancel** button.

The selected framework will display in the **Create Associations** frame.

.. image:: static/OpenSALT_User_Manual_148.png
   :height: 249 px
   :width: 624 px


Select the item from the right by clicking on it and dragging it over the associated item on the left.

.. image:: static/OpenSALT_User_Manual_149.png
   :height: 261 px
   :width: 624 px


The Create Association window will display showing the item that was both dragged and dropped as well as the item that it was connected to.

.. image:: static/OpenSALT_User_Manual_150.png
   :height: 172 px
   :width: 548 px


The user can select the **Relationship Type** from the drop down and change the relationship arrow as needed by clicking on the **Switch** button.

.. image:: static/OpenSALT_User_Manual_151.png
   :height: 181 px
   :width: 584 px


To save the association, click the **Associate** button.

To cancel and abandon the association, click the **Cancel** button.

The **Framework Display** page will refresh. If the user clicks on the item in the **Framework Display** and then clicks **Item Details** , the newly created association will be visible.

.. image:: static/OpenSALT_User_Manual_152.png
   :height: 252 px
   :width: 624 px


To add several of the same type of association to one item, the user can open the multi select function by clicking on the empty checkbox above the framework displayed in the **Create Associations** frame.

.. image:: static/OpenSALT_User_Manual_138.png
   :height: 116 px
   :width: 289 px


The user can now check one or more boxes and click on an item to drag and drop to the left. All items selected will become part of the association. Note if a Parent is selected all the children will associate even if they are not individually checked.

.. image:: static/OpenSALT_User_Manual_153.png
   :height: 189 px
   :width: 624 px


When the users drags the items to the the left and associates them with an item, the **Create Associations** window will display. The user will note that the list will only display the first of the associated item, and will indicate there are additional items selected. Also note all items will have the same association, as you can only select one association type. Set the associations as required and click the Associate button.

.. image:: static/OpenSALT_User_Manual_154.png
   :height: 212 px
   :width: 624 px


Note to close the multi select function, click on **Actions** and select **Hide Checkboxes**.

.. image:: static/OpenSALT_User_Manual_140.png
   :height: 186 px
   :width: 293 px


.. _hd1b6e2e5a1562f4f60da1a3f1f60:

6.6.1.2 Edit Associations
^^^^^^^^^^^^^^^^^^^^^^^^^^

To Edit an association, the user must delete the association and create a new association. PLease see section \ |LINK20|\  for how to delete an association and \ |LINK21|\  for how to create a new association.

.. |LINK20| raw:: html

    <a href="#heading=h.snby2z2ysyqp">6.6.1.2</a>

.. |LINK21| raw:: html

    <a href="#heading=h.w21k7kyd2nwq">6.6.1.1</a>

.. _h3465b16792e30151f3c47675d20f4c:

6.6.1.2 Delete Associations
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Users can either use the **Tree View** or the **Association View** to delete associations.

6.6.1.2.1 Delete Associations from Tree View

On the **Framework Display** page, click on the **Tree View** button if not already selected. Then locate the association in the I**tem Detail** frame. Click the **X** icon next to the association to remove.

.. image:: static/OpenSALT_User_Manual_155.png
   :height: 334 px
   :width: 624 px


The user will get a popup window warning that he action can not be undone. If the user wants to proceed and delete the association, the user will click the **OK** button. Otherwise the user can cancel by clicking on the **Cancel** button.

.. image:: static/OpenSALT_User_Manual_156.png
   :height: 133 px
   :width: 429 px


6.6.1.2.2 Delete Associations from Association View

On the **Framework Display** page, click on the **Association View** button if not already selected.

.. image:: static/OpenSALT_User_Manual_157.png
   :height: 296 px
   :width: 624 px


Locate the association in the in the list to be deleted. Click the **X** icon next to the association to remove.

.. image:: static/OpenSALT_User_Manual_158.png
   :height: 390 px
   :width: 624 px


The user will get a popup window warning that he action can not be undone. If the user wants to proceed and delete the association, the user will click the **OK** button. Otherwise the user can cancel by clicking on the **Cancel** button.

.. image:: static/OpenSALT_User_Manual_156.png
   :height: 133 px
   :width: 429 px


.. _h48482a61264d7437205d1a12f3f3d6b:

6.6.2 Association Groups
~~~~~~~~~~~~~~~~~~~~~~~~

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

Associations can belong to an association group. There is a selector to filter the view for only those items and associations for a specific group, if there are any. If there are no group, all associations belong to the default “Null” group. If there are any association group, the default view is “All” association groups. The Association group filter drop list allows you to choose the “null” group, the “All” group or any specific group. In the view, an association that belongs to an association group is tagged in the display as such:

On the **Framework Display** page, click the **Manage Association Groups** button in the **Item Detail** frame.

.. image:: static/OpenSALT_User_Manual_159.png
   :height: 269 px
   :width: 558 px


The **Manage Association Groups** window will display. Click on the **Add a New Association Group** button.

.. image:: static/OpenSALT_User_Manual_160.png
   :height: 245 px
   :width: 624 px


The **Add New Association Group** window will display. The user will need to enter a **Title** and the optional **Description**. Next click on the **Create** button.

.. image:: static/OpenSALT_User_Manual_161.png
   :height: 284 px
   :width: 624 px


The user will repeat the process to add any needed **Association Groups**.

.. image:: static/OpenSALT_User_Manual_162.png
   :height: 321 px
   :width: 624 px


After creating the required Association Groups, the user can **Edit** a Group, **Delete** a Group or click **Done**.

The filter option for the **Association Groups** will now display on the **Display Frameworks** page.

.. image:: static/OpenSALT_User_Manual_163.png
   :height: 313 px
   :width: 520 px


The user will now need to associate items with the appropriate groups.


.. _h6fe4164b12672914514d4f13492564:

Note that association groups do not currently import correclty to others instances of OpenSALT 2.2.

6.6.3 Crosswalk Associations
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor**

OpenSALT allows for users to create crosswalks between frameworks. To create a crosswalk the user will need to start with an empty framework. For instructions on creating a framework see section \ |LINK22|\ .

.. |LINK22| raw:: html

    <a href="#heading=h.uzlj2tpaic68">6.2.2</a>

How-To `Video
<https://youtu.be/eU8dEE2dzr8>`_

.. _h3123662d575a5b54732475fd62e:

6.6.3.1 Create Crosswalk Associations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Open the framework to the **Display Framework** page. In the click on **Change Document** to select the first framework to use in the crosswalk.

.. image:: static/OpenSALT_User_Manual_164.png
   :height: 244 px
   :width: 624 px


This will open a Document dropdown. The user can select a framework that is in their current OpenSALT server from the list by clicking on the desired framework.

.. image:: static/OpenSALT_User_Manual_165.png
   :height: 345 px
   :width: 624 px


Alternatively the user can connect to a framework that is outside their system by selecting the final option: **Load an “external” document by url…** This allows the user to select any CASE compliant framework that is stored on an external location.

The **Load External Document** window will display. The user will need to copy and paste, or type in the url for the Case-compliant framework.

.. image:: static/OpenSALT_User_Manual_145.png
   :height: 186 px
   :width: 568 px


In instances of OpenSALT, the **Case Framework URL** can be found on the **Framework Display** page in the **Item Detail** frame.

.. image:: static/OpenSALT_User_Manual_146.png
   :height: 170 px
   :width: 624 px


Note if the copied URL does not have the .JSON extension, you will need to add it for the document to load.

.. image:: static/OpenSALT_User_Manual_147.png
   :height: 204 px
   :width: 624 px


To load the framework, click the **Load Document** button.

Next the user will click on the **Create Association** option above the **Item Detail** frame.

.. image:: static/OpenSALT_User_Manual_166.png
   :height: 234 px
   :width: 624 px


A Document dropdown will display to allow the user to select the second framework to be selected. Again the user can select an existing framework from their OpenSALT server or can select an outside CASE-compliant framework.

.. image:: static/OpenSALT_User_Manual_167.png
   :height: 284 px
   :width: 624 px


The user can now use drag and drop to select items from the right and drag to connect to items on the left to establish the cross walk. After an association is connected with the drag and drop, the Create Association window will display and the user can define the association.

.. image:: static/OpenSALT_User_Manual_168.png
   :height: 181 px
   :width: 570 px


When the user is satisfied with the association definition, click on the **Associate** button.

To cancel, click on the **Cancel** button.

The user should repeat this process to connect all required framework items for the crosswalk.

To view the cross walk, the user will click on the **Association View** at the top of the screen.

.. image:: static/OpenSALT_User_Manual_169.png
   :height: 180 px
   :width: 624 px


.. image:: static/OpenSALT_User_Manual_170.png
   :height: 313 px
   :width: 624 px


.. _h0571ea6415539114494f5a71425a:

6.6.3.2 Edit Crosswalk Associations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To Edit a crosswalk association, the user must delete the associations and create new associations. Please see section \ |LINK23|\  for how to delete an association and \ |LINK24|\  for how to create a new association.

.. |LINK23| raw:: html

    <a href="#heading=h.snby2z2ysyqp">6.6.1.2</a>

.. |LINK24| raw:: html

    <a href="#heading=h.w21k7kyd2nwq">6.6.1.1</a>

.. _h5d772b55c793e1c441729195453c14:

6.6.3.3 Delete Crosswalk Associations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

On the **Framework Display** page, click on the **Association View** button if not already selected.

.. image:: static/OpenSALT_User_Manual_169.png
   :height: 180 px
   :width: 624 px


Locate the association in the in the list to be deleted. Click the **X** icon next to the association to remove.

.. image:: static/OpenSALT_User_Manual_170.png
   :height: 313 px
   :width: 624 px


The user will get a popup window warning that he action can not be undone. If the user wants to proceed and delete the association, the user will click the **OK** button. Otherwise the user can cancel by clicking on the **Cancel** button.

.. image:: static/OpenSALT_User_Manual_156.png
   :height: 133 px
   :width: 429 px


Alternatively if the entire crosswalk needs to be deleted and all associations, the user can delete the framework instead of removing all associations. Please see section \ |LINK25|\  for instructions on deleting a framework.

.. |LINK25| raw:: html

    <a href="#heading=h.z5n3wwx83avg">6.8</a>

.. _h783d576b5c1c507f6d718562d5c5:

6.7 Export Frameworks Packages
-------------------------------

**Audience: Super Users, Super Editor, Organization Admins, Organization Editor, Public**

OpenSALT is designed to enable all users roles to **Export** complete framework packages or documents. While **Public** users can only export framework packages that are in an **Adopted**, **Draft**, or **Depreciated** release status, credentialed users will have the ability to export **Draft** and **Private Draft** framework packages as well.

To **Export** a framework package the user needs to be on the **Framework Display** page for the selected framework and then click on the **Export** button.

.. image:: static/OpenSALT_User_Manual_171.png
   :height: 194 px
   :width: 624 px


An Export window will display to provide the user with several **Export** options:

* Competency Framework Package (JSON)

* Styled PDF

* Spreadsheet Export

* HTML Archive

* Direct OpenSALT Link

.. image:: static/OpenSALT_User_Manual_172.png
   :height: 229 px
   :width: 573 px


The user can select an **Export** option or can click on the **Done** button or the ‘**X**’ at the top of the window  to close the **Export** window. Each **Export** type will be discussed in the following subsections.

.. _h163e401e8291001a4c5447e45136c:

6.7.1 Export Competency Framework Package (JSON) File
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The first **Export** option is the **Competency Framework Package (JSON)**. This option allows users to extract the data for the framework packaging in the JavaScript Object Notation (JSON) file format. This is a lightweight, text-based, language-independent data interchange format that allows for easy ingestion into other system and applications using a common standard programming language.

When a user mouses over the **Competency Framework Package (JSON)** button, a soft explanation is displayed that advises the user of the button’s intended purpose: ‘Exports a JSON file using the IMS-standard format. This is the best format to user for Archiving Frameworks.’

.. image:: static/OpenSALT_User_Manual_173.png
   :height: 249 px
   :width: 624 px


To generate a JSON file for the Framework Package, the user will click on the **Competency Framework Package (JSON)** *button.* The browser will automatically create and down load a JSON file for the Framework Package. The user will need to retrieve the file following the browser’s specific protocol and path. The image below shows the download in Chrome. Note the file is in the download frame at the bottom of the page. It has also been added to the user’s Download folder within the user’s My Documents.

.. image:: static/OpenSALT_User_Manual_174.png
   :height: 270 px
   :width: 624 px

To open the JSON file the user will need to identify a compatible application on their computer. Notepad or NotePad ++ can be used if no preferred application is identified.

The following is an example of the generated JSON file viewed in Notepad.

.. image:: static/OpenSALT_User_Manual_175.png
   :height: 200 px
   :width: 505 px


.. _h69105f5c3a80644f6a806369c586458:

6.7.2 Export Styled PDF (Future Function)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The second **Export** option is the **Styled PDF** button.

.. image:: static/OpenSALT_User_Manual_176.png
   :height: 249 px
   :width: 624 px


The purpose of this **Export** option is to produce a system generated **PDF** with nice formatting and styling that can be used to compare against a source document for validation or can replace source documentation as needed.

Users will note that at this time the button is not active. A description will not display when a user mouses-over the button, nor will the button respond with clicked. This is a placeholder for future functionality. As of the current release of OpenSALT this feature is not available. Though it is on the road map and is expected to be in a future release. If any organization requires this functionality, you can sponsor the development of the feature to help prioritize the development timeline by contacting PCG, ACT, or School City to discuss development costs and your needs.

.. _h596b20112477664e57757b30727b58:

6.7.3 Export Spreadsheet
~~~~~~~~~~~~~~~~~~~~~~~~

The third **Export** option is the **Spreadsheet Export.** This option allows users to extract the data for the framework packaging in a spreadsheet file that can be opened/viewed/edited in a program like Microsoft’s Excel or Google Sheets.

When a user mouses over the **Spreadsheet Export** button, a soft explanation is displayed that advises the user of the button’s intended purpose: ‘Exports as an Excel spreadsheet file that you can open and edit in spreadsheet programs such as Microsoft Excel. ’

.. image:: static/OpenSALT_User_Manual_177.png
   :height: 249 px
   :width: 624 px


To generate a spreadsheet file for the Framework Package, the user will click on the **Spreadsheet Export** *button.* The browser will automatically create and download a case xlsx file for the Framework Package. The user will need to retrieve the file following the browser’s specific protocol and path. The image below shows the download in Chrome. Note the file is in the download frame at the bottom of the page. It has also been added to the user’s Download folder within the user’s My Documents.

.. image:: static/OpenSALT_User_Manual_178.png
   :height: 269 px
   :width: 624 px


To open the spreadsheet file the user will need to identify a compatible application on their computer. The most common applications used are Microsoft Excel or Google Sheets.

Users credentialed users who are experienced with importing Frameworks into OpenSALT with the CASE template will already be familiar with this spreadsheet format. For all other users, the following details the exported spreadsheet file.

When opened the spreadsheet file will have three tabs:

#. CF Doc

#. CF Item

#. CF Association

.. image:: static/OpenSALT_User_Manual_179.png
   :height: 62 px
   :width: 292 px


.. _h2c3d432f26522266f31614d703c15b:

6.7.3.1 CF Doc Tab
^^^^^^^^^^^^^^^^^^

The purpose of the first tab, CF Doc, is to provide the user with basic background information on the Framework Package.

.. image:: static/OpenSALT_User_Manual_180.png
   :height: 61 px
   :width: 829 px


The columns on the spreadsheet include the following:

* *Identifier:*  The identifier is intended to be used as the primary key global identifier within or external to the system. This is a mandatory field in OpenSALT and the export will contain data.

* *Creator:*  The entity that authorized or created the competency framework. It could be an education agency, higher education institution, professional body. It is the owner of the competency framework (e.g CCSSO, TEA, NGSS). This is a mandatory field in OpenSALT and the export will contain data.

* *Title*: The title as it appears on the cover of the Official Source artifact, although it may be a title created by the Publisher. This is a mandatory field in OpenSALT and the export will contain data.

* *LastChangeDateTime:* The field is used to establish any change, not just major version revisions. This is a mandatory field in OpenSALT and the export will contain data.

* *OfficialsourceURL*:  The URL of the artifact adopted by the Standard Setting Entity. Often this document is published in html and/or as pdf and is used by the standard setting entity as part of its approval process. Since it is not the intent of this specification to fully reproduce the human-facing content and formatting of the source document, it is recommended that this document be transmitted as part of the competency framework package. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Publisher:*  The entity that loads and publishes the Framework. Note that in  many cases, the Standard Setting Entity may lack technical capabilities to publish the Competency Framework in a standard format so a third party may be displayed. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Description:*  The description is typically created by the the Publisher as a standard description of the Competency Framework.This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Subject:* This is a string expressing the general subject area of the Competency Framework (e.g. Mathematics). This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Language:* HTML Language Country Code VIA- country code from \ |LINK26|\ . This is an optional field in OpenSALT. If best practices are not followed, this field may be blank. However OpenSALT assumes English if not other language value is entered.

.. |LINK26| raw:: html

    <a href="https://tooCF.ietf.org/html/bcp47" target="_blank">https://tooCF.ietf.org/html/bcp47</a>

* *Version:* This is used to separate any version information expressed by the Official Source artifact. Once and CF Pkg has been approved and published, any changes to an CF Item will constitute a new version of the CF Doc. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *AdoptionStatus:* Adoption status displays the Framework's current status as Draft, Private, Draft,  Adopted, or Deprecated.  OpenSALT assumes Adopted as the default if no status is specifically selected for the framework. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank. OpenSALT assumes Adopted as the default if no status is specifically selected for the framework.

* *StatusStartDate:* The date that the CF Doc status started. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *StatusEndDate:*  This date is often only known when a new status is started. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *License:* Systems may filter for content with particular licences to support discovery. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *Notes:* Notes or comments generated by the Framework Publisher about the context of the Framework. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

.. _h495651a32261e342218226c7b239:

6.7.3.2 CF Item Tab
^^^^^^^^^^^^^^^^^^^

The purpose of the second tab, CF Item, is to provide the user with items and content within the Framework Package.

.. image:: static/OpenSALT_User_Manual_181.png
   :height: 332 px
   :width: 624 px


The columns on the spreadsheet include the following:

* *Identifier:*  The identifier is intended to be used as the primary key global identifier within or external to the system. This is a mandatory field in OpenSALT and the export will contain data.

* *FullStatement*: The the main content of the CF Item. It is used to express both nodes and granular statements. If the statement is part of a list, the list enumeration should not be included in the statement and should instead be contained in the List Enumeration in Source Document. This is a mandatory field in OpenSALT and the export will contain data.

* *HumanCodingScheme*: The ID sometimes used by humans to identify a CF Item. It often will use concatenated codes expressing its position in the taxonomy and abbreviations to convey other classification information (e.g. K.CC.1.1). This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *SmartLevel:*   This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *ListEnumeration:* Used to parse out enumerations or bullets that precede CF Item statements. This is an optional field in OpenSALT. If best practices are not followed, this field may be blank.

* *AbbreviatedStatement:* Abbreviated or summary statement provided by the Publisher. This is an optional field in OpenSALT and may be blank.

* *ConceptKeywords:* Upper level CF Item node statements may be used to populate Concept Keywords of lower level nodes. upper The concepts data structure allows a master list of keywords to be defined which can then be parsed down specific to a node. This works as usually concepts will be a less granular hierarchy representation of of the more detailed nodes in CF items. A node could be 'Geometry' and the lower node is 'Tangents' but the keywords for 'tangents' could include the word geometry. This is an optional field in OpenSALT and may be blank.

* *Notes:* In some cases, this can be used to contain additional information found in the original source document. This is an optional field in OpenSALT and may be blank.

* *Language:* HTML Language Country Code VIA- country code from \ |LINK27|\ . This is an optional field in OpenSALT. If best practices are not followed, this field may be blank. However OpenSALT assumes English if not other language value is entered.

.. |LINK27| raw:: html

    <a href="https://tooCF.ietf.org/html/bcp47" target="_blank">https://tooCF.ietf.org/html/bcp47</a>

* *EducationLevel:* 	The current US K12 defined vocabulary is to use CEDS https://ceds.ed.gov/cedselementdetaiCF.aspx?termid=8267. Multiple values are allowed via comma delimitation and should be used to express grade spans. This is an optional field in OpenSALT and may be blank.

* *CFItemType:* e.g., "Standard," "Benchmark," "Strand," or "Topic." or "Level 1, Level 2,..." This is an optional field in OpenSALT and may be blank.

* *License:* Systems may filter for content with particular licences to support discovery. This is an optional field in OpenSALT and may be blank.

* *LastChangeDateTime:* This is used for versioning. This is a mandatory field in OpenSALT and the export will contain data.

.. _h7a453f1eb35d645b3d574c4e4a2552:

6.7.3.3 CF Association Tab
^^^^^^^^^^^^^^^^^^^^^^^^^^

The purpose of the third tab, CF Association, is to provide the user with items and content within the Framework Package.

.. image:: static/OpenSALT_User_Manual_182.png
   :height: 337 px
   :width: 417 px


The columns on the spreadsheet include the following:

* *Identifier:*  The identifier is an unambiguous, synthetic, unique reference to the association. This is a mandatory field in OpenSALT and the export will contain data.

* *URI:*  Establishes uniqueness of an association between a learning standard and another learning standard or other objects such as learning resources. [CEDS Element: Learning Standard Item Association Identifier URI, ID:000871].  This is a mandatory field in OpenSALT and the export will contain data.

* *OriginNodeIdentifier:* Identifier of the origin node when the Learning Standard Item Association is used as a connector in a learning map. [CEDS Element: Learning Standard Item Association Origin Node URI, ID: 001406]. This is a mandatory field in OpenSALT and the export will contain data.

* *DestinationNodeIdentifier:* Identifier of the destination node when the CF Association is used as a connector in a learning map. [CEDS Element: Learning Standard Item Association Destination Node URI, ID: 001404]. This is a mandatory field in OpenSALT and the export will contain data.

* *AssociationType:* A controlled vocabulary used to express the types of associations used to describe the relationship between CF Docs and between CF Items. This is a mandatory field in OpenSALT and the export will contain data.

* *AssociationGroupIdentifier:*  An identifier to allow associations to be grouped together. Different values only have to be unique within the document. This is an optional field in OpenSALT and may be blank.

* *AssociationGroupName:*  A common group name to allow associations to be grouped together. Different values only have to be unique within the document. This is an optional field in OpenSALT and may be blank.

* *LastChangeDateTime:* A system generated log of the most recent change to this record. This is a mandatory field in OpenSALT and the export will contain data.

.. _h637197e5b246b4c3f7c222d352d67:

6.7.4 Export HTML Archive (Future Function)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The fourth **Export** option is the **HTM Archive** button.

.. image:: static/OpenSALT_User_Manual_183.png
   :height: 248 px
   :width: 624 px

The purpose of this **Export** option is to produce an **HTML** code snippet that can be used on an alternative website that renders the framework in a consistent manner to the display on OpenSALT.

Users will note that at this time the button is not active. A description will not display when a user mouses-over the button, nor will the button respond with clicked. This is a placeholder for future functionality. As of the current release of OpenSALT this feature is not available. Though it is on the road map and is expected to be in a future release. If any organization requires this functionality, you can sponsor the development of the feature to help prioritize the development timeline by contacting PCG,ACT, or School City to discuss development costs and your needs.

.. _h74c126565a611e731014cb6b8:

6.7.5 Link for Browser View
~~~~~~~~~~~~~~~~~~~~~~~~~~~

The final share option to connect to the Framework Package outside of OpenSALT is the **Browser Link**.

.. image:: static/OpenSALT_User_Manual_184.png
   :height: 249 px
   :width: 624 px


OpenSALT provides the users with the direct **URL** for the selected Framework Package as both a **hyperlink** and display the text of the unique **URL**. The sure can copy the **URL** to us in any document, application or website. The **URL** will return the audience to the selected **Framework’s Display** page within OpenSALT when followed. Any user will be able to access the selected Framework package as no credentials or login are required when following the URL link.

.. _h3e237e1a4d5b2d787d76433f407b725f:

7.0 Options
===========

.. _h366f59222a45735257254b1927547c6a:

7.1 Commenting Module
---------------------

	Published frameworks are able to be commented on by authenticated users for the purpose of collecting feedback on framework item metadata.  Commenting must be turned on by a system administrator.

.. _h7b36562d3c294c5a7d537c95a1a6c59:

7.1.1 Features
~~~~~~~~~~~~~~

	Provisioned users are able to upvote and reply to other users comments. You are able to delete comments that you have written as well. Simply navigate to any framework item and make your comment, or upvote/respond to others previous comments. The comment panel may be hidden - it will be on the bottom of the ride side panel.

.. image:: static/OpenSALT_User_Manual_185.png
   :height: 262 px
   :width: 624 px


.. _h32706aa7115195a6b334365a5d5e41:

7.1.2 Viewing Comments
~~~~~~~~~~~~~~~~~~~~~~

You are able to sort comments by the three tabs - newest, Oldest, and Most Popular (see graphic above). You may use these tabs to sort comments in the way that suits your interest and purpose best. Comments are not a part of the framework itself but independently stored. Due to a feature that truncates the email address of a participant, users cannot start their usernames with the @ symbol.

.. image:: static/OpenSALT_User_Manual_186.png
   :height: 278 px
   :width: 484 px


.. _h49416333194b564671d134e68507a60:

7.1.3 License
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

OpenSALT has integrated this third party code ( http://viima.github.io/jquery-comments/ )with a congruent MIT license in order for reviewing frameworks.

.. _h662f65664e775a707382e4d3e1c37:

7.2 User Account Self-Creation
------------------------------

.. _h5cc5056584c262f761b5b2746a3437:

7.2.1 Features
~~~~~~~~~~~~~~

Users have the ability to create their own accounts and organizations on signup.

.. _h5cc5056584c262f761b5b2746a324a:

7.2.2 Process
~~~~~~~~~~~~~

#. Select “Sign up” from the top right page or Log In page.

.. image:: static/OpenSALT_User_Manual_187.png
   :height: 85 px
   :width: 218 px


#. User enters their desired email address and password (twice). They cannot enter an email address already in use and their passwords must match.

.. image:: static/OpenSALT_User_Manual_188.png
   :height: 165 px
   :width: 624 px


#. They also can select their Organization and if no Organization exists, create one.

.. image:: static/OpenSALT_User_Manual_189.png
   :height: 148 px
   :width: 625 px

Upon submitting this information a short email is sent notifying the user of a pending account status.

4. Once the Super Admin receives an email notification, they can navigate to the User List page and Approve or Suspend/Reject the user.

.. image:: static/OpenSALT_User_Manual_190.png
   :height: 148 px
   :width: 624 px

Rejecting the users will simply suspend the accounts. Accepting the user will generate another confirmation email to the users notifying them of successful account creation,

.. _j5cc5056584c262f761b5b2746a346o:

7.2.3 Configuration
~~~~~~~~~~~~~~~~~~~
$. System Administrators can turn this feature on or off as well as email addresses/text in their parameters.yml file to "always-on" then restart docker. You must also enable the email server. This change triggers the Create Account button as well as allows user access to the Create account page and shows Pending users on User List page.
More information: \ |LINK28|\

.. |LINK28| raw:: html

    <a href="https://github.com/opensalt/opensalt/blob/develop/docs/CONFIGURATION.md" target="_blank">https://github.com/opensalt/opensalt/blob/develop/docs/CONFIGURATION.md</a>

.. _j5cc5056584c262f761b5b2746a3460:

7.3 Additional Fields
~~~~~~~~~~~~~~~~~~~~~

OpenSALT 2.2 has the ability to add additional fields to the CfItem entity. These fields will NOT be exported with a standard CASE export or visible via the API. They will however be viewable when editing the Cf Item of any framework on that OpenSALT instance and be exported/able to be updated via the Spreadsheet Updater.

To view the additional fields, login and a super user and go to <server name>/additional_field eg frameworks.act.org/additional_field

.. image:: static/add_field_screen.png

To create a new field, select New and create your field.

.. image:: static/add_field.png

The video below shows this as well as offering best practices guidance.
\ |LINK29|\

.. |LINK29| raw:: html
<a href="https://www.youtube.com/watch?v=7pHAMh8QfJk&list=PLc37jyWQOZ2aLZ1tL3lTiPlti699qsobN&index=5&t=0s" target="_blank">Additional Fields Feature Video</a>

.. _j5cc5056584c262f761b5b2746a3461:

7.4 File Storage and Image Attachment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Often users want to attach an image to the notes section for clarity, or perhaps fullStatement can point to a learning object etc. The ability to add uploads and images was created for this type of functionality.

7.4.1 Configuration
While files cannot be stored natively in the CASE JSON, OpenSALT allows administrators setting up OpenSALT to include an AWS bucket as well as a prefix in the docker-compose.yml file - then the images are inserted with the native markdown/attachments are linked. Make sure your bucket is public if you intend for the CASE framework to be shared and disseminated publicly.

AWS_ACCESS_KEY_ID:
AWS_SECRET_ACCESS_KEY:
AWS_S3_BUCKET:
AWS_S3_REGION:
AWS_S3_PREFIX:
ATTACHMENT_URL_PREFIX:
BUCKET_PROVIDER:

7.4.2 Usage

Users may drag and drop and image into the fullStatement and Notes field when this functionality is enabled. Future plans would add it to Exemplar as well but that is not on the OpenSALT roadmap at this time.
