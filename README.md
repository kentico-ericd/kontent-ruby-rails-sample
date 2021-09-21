[![Konten Discord](https://img.shields.io/discord/821885171984891914?color=%237289DA&label=Kontent%20Discord&logo=discord)](https://discord.gg/SKCxwPtevJ) [![Stack Overflow](https://img.shields.io/badge/Stack%20Overflow-ASK%20NOW-FE7A16.svg?logo=stackoverflow&logoColor=white)](https://stackoverflow.com/tags/kentico-kontent)


# Kontent Rails Sample Application

This basic Rails application demonstrates how to create a Rails application using the [Kontent Ruby SDK](https://github.com/Kentico/kontent-delivery-sdk-ruby) and a [sample project](https://docs.kontent.ai/tutorials/manage-kontent/projects/manage-projects#a-create-a-sample-project).

See [Build your first Ruby on Rails app](https://docs.kontent.ai/tutorials/develop-apps/get-started/build-your-first-app?tech=ruby) for a detailed walkthrough of how the sample application was developed.

![Screenshot](/screenshot.png)

## Install & Run

1. Clone the repository
1. Run `bundle install`
1. Open the __app/controllers/application_controller.rb__ file and set your project ID on this line:  
`PROJECT_ID = '<your-project-ID>'.freeze`
1. Run `rails server`. Your application will be accessible at __localhost:3000__

## Features

- Loads articles from Kontent asynchronously via [render_async](https://github.com/renderedtext/render_async)
- Rich text component rendering via [`InlineContentItemResolver`](https://github.com/Kentico/kontent-delivery-sdk-ruby#resolving-inline-content)
- Content item link resolution via [`ContentLinkResolver`](https://github.com/Kentico/kontent-delivery-sdk-ruby#resolving-links)