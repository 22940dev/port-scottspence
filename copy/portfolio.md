<script>
  import DateUpdated from '$lib/components/date-updated.svelte'
  import Small from '$lib/components/small.svelte'
  import TopLanguages from '$lib/components/top-languages.svelte'
  import GitHubContributions from '$lib/components/github-contributions.svelte'
  import Projects from '$lib/components/portfolio-projects.svelte'
</script>

## Portfolio

<Small>
  Last updated: <DateUpdated date='2021-01-09' small='true' />
</Small>

This page details some projects I have worked on along with my GitHub
contributions.

The charts are made using a serverless function to query the GitHub
GraphQL API. The serverless function uses [Google charts] to render
the data then Puppeteer to take a picture of the chart and return it
as an image. Clicking on one of the charts will open the chart in
interactive mode where you hover over the elements for more
information.

### Top Languages used:

Here's my top languages I use, calculated from my GitHub commits.

This chart is updated via the GitHub GraphQL endpoint every time the
page is requested, you can see what languages I'm working with daily.

<TopLanguages />

### Projects:

A mixture of personal and professional projects I have worked on. If
you want to collaborate on anything reach out. 👍

<Projects />

### Contributions:

This is my GitHub contributions chart taken from the GitHub API
GraphQL endpoint. You can click on it to see the interactive example.

<GitHubContributions />

---

[google charts]: https://developers.google.com/chart/interactive/docs
