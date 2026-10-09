# Two-Tier Architecture

## What Is a Two-Tier Architecture?

A two-tier architecture is an application design that separates a system into two main parts: the web/application tier and the database tier. These tiers communicate with each other to provide application services and store information.

## The Web/Application Tier

The web/application tier handles user interactions and HTTP requests. In this laboratory, Nextcloud provides the web interface that allows users to access and manage their files through a browser.

## The Database Tier

The database tier stores persistent information required by the application. MariaDB stores Nextcloud data such as user account information, file metadata, and application settings.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to maintain, troubleshoot, and scale. It also allows each service to be managed independently and reduces the need to configure both services inside a single container.
