# Alterforms
Custom Module for Drupal 8

## Description
Custom Module for Drupal 8: getting the form ID by messages and changes through hooks like form_alter or FORM_ID_alter.

## Purpose
This module is only for development environments (disable / uninstall before moving to other environments).

## Context
Do you want to make changes in a form in Drupal 8 and you need to extract its form ID? This module, once installed and activated, configures a Drupal-styled message with the id of each form that appears on your website. Only when you open it will you be able to see its ID in the header.

## Install
Only get this url and use wget from your prompt. Move the folder within /your_drupal8/modules/ or /your_drupal8/modules/custom. 

After that, only active the module under /admin/extend/modules, section "Development".

![Alterforms Drupal 8](https://github.com/davidjguru/alterforms/blob/master/images/alterforms_drupal_8_module_install.png)

## Using the module
This module have a alterforms.module file with a central function, a classic hook called "alterforms_form_alter" based in hook_form_alter. 


