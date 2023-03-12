# [pocroianu]

This is a blog website created using [Hugo](https://gohugo.io/) and hosted on [GitHub Pages](https://pages.github.com/). 

## Getting Started

### Prerequisites

Before you start, you will need to have the following tools installed on your machine:

- [Git](https://git-scm.com/)
- [Hugo](https://gohugo.io/getting-started/installing/)

### Installation

1. Clone the repository:
`git clone https://github.com/[username]/[repository-name].git`

2. Navigate to the project folder:
`cd [repository-name]`

3. Start the Hugo server:
`hugo server`

4. Open your web browser and navigate to `http://localhost:1313`.

### Configuration

To customize the website, you can modify the configuration file `config.toml`.

## Usage

### Creating a new post

To create a new blog post, run the following command:
`hugo new posts/[post-name].md`

This will create a new Markdown file in the `content/posts` folder.

### Deploying the website

To deploy the website to GitHub Pages, run the following command:
`./deploy.sh`

This will generate the static HTML files and push them to the `gh-pages` branch of the repository.

## License

This project is licensed under the [MIT License](LICENSE).
