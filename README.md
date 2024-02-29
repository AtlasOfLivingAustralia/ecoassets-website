# Ecoassets Quarto website

EcoAssets brings together environmental data collected from three national research infrastructures – the Atlas of Living Australia (ALA), the Integrated Marine Operating System (IMOS) and the Ecosystem Research Infrastructure (TERN).

The current website(https://ecoassets.org.au/) is a static WordPress site that explains the project and provides access to the aggregated EcoAssets datasets. 

Over the summer (December 2023-February 2024), I worked as a vacation student at the ALA on a project to revamp the current ecoAssets website, transitioning from the static site to a visually appealing Quarto site capable of embedding interactive elements. The idea was to have a generous and interesting interface to the data, so that users can understand the scale of the data and learn how to use it. 

More information about the project and findings can be found in ClaraProjectSummary.qmd

In the design process, I first created high-fidelity Figma mockups (https://www.figma.com/file/HKJsBaRj9so7UfeQTuzSUl/EcoAssets?type=design&node-id=0%3A1&mode=design&t=pbNoO4C0n9uLHLps-1). 

Then I created this Quarto website prototype. The website includes:
- index.qmd: the homepage
- about.qmd; About the EcoAssets project
- data.qmd: About the data in EcoAssets (WIP)
- monitoring_data.qmd: Explanation of the monitoring data in EcoAssets (WIP)
- biodiversity_data.qmd: Explanation of the biodiversity in EcoAssets, with a visualisation (WIP)
- news.qmd: a news page with news posts located in /posts
- 404.qmd
- Some html:
  - a back-to-top button
  - a title-block.html that removes the title-block for .qmd pages on the site
  - a progress-bar for scrollystories
  - a custom footer for the site

Website styling is located in styles/theme.scss . 

Some scrollytelling attempts are also included in /stories. These are all a work in progress:
- dataStory0.qmd: A simple data story showing how scrollama works, also starting to explore scrollyteller implementation. 
- d3Chart.qmd: d3 and JavaScript experiments to test how ObservableJS blocks work in Quarto. 
- exampleStory.qmd: An attempt to recreate the scrollyteller.js tutorial example for the Wealth and Health of Nations chart. 
- ECharts.qmd: An Echarts example of how to embed Echarts in Quarto (not fully implemented as it requires python).
- ecoAssetsDataStory.qmd: A simple EcoAssets data story, explaining the project and visualisations (WIP). 

Overall, the website still needs more work in terms of testing responsiveness and ensuring accessibility. 
