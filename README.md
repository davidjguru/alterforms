# Alterforms
Custom Module for Drupal 8

## Description
Custom Module for Drupal 8: getting all the info about your forms within Drupal 8 project like the form ID, fields and others.
It offers a simple workspace to add changes and modifications to your forms through a simple if-else structure, as a simple and centralized way of operating on forms.


## Purpose
The first goal is to facilitate the daily work on forms in Drupal 8: create and modify through a quick learning of FormAPI.
This module is only for development environments (disable / uninstall before moving to other environments).

## Context
Do you want to make changes in a form in Drupal 8 and you need to extract its form ID? This module, once installed and activated, configures a Drupal-styled message with the id of each form that appears on your website. Only when you open it will you be able to see its ID in the header.
In a complementary way you can also use its debugging functions to extract all the information available from each form: actions, content, states and fields.

## Install
Only get this url and use wget from your prompt. Move the folder within /your_drupal8/modules/ or /your_drupal8/modules/custom. 
Alterforms has dependencies: Kint (sub-module of Devel) and this depends on the installation of the Devel suite. It is also necessary to install Devel completely using the normal methods (composer, drush, wget or interface).
After that, only active the module under /admin/extend/modules, section "Development".

![Alterforms Drupal 8](https://github.com/davidjguru/alterforms/blob/master/images/alterforms_drupal_8_module_install.png)

## Using the module
This module have a alterforms.module file with a central function, a classic hook called "alterforms_form_alter" based in hook_form_alter. 

To visualize all the information of a form, you have two information dump functions on screen, you only have to use one (comment the line you do not want to use), at the foot of the hook form alter: var_dump() and kint().

By opening the file alterforms.module with your favorite text editor, you can see the code and select the debugging function.
![Funcions Alterforms](https://github.com/davidjguru/alterforms/blob/master/images/alterforms_drupal_8_module_select_debugging_functions.png)

Going to your Drupal project through your browser, access the URL of the chosen form and you will see in the header all the rendered information.
![Info Alterforms](https://github.com/davidjguru/alterforms/blob/master/images/alterforms_drupal_8_module_info_forms.png)


