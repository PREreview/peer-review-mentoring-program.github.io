# PREreview Peer Review Mentoring Program

***Sharing. Connecting. Empowering***

## Welcome!

First and foremost, Welcome! 🎉 Willkommen! 🎊 Bienvenue! 🙏 सुस्वागत (Suswagat)🎈🎈🎈

This document (the `README` file) is a hub to give you some information about the
project. Jump straight to one of the sections below, or just scroll down to find
out more.

## What are we doing?

We are working to build a free cohort-based mentoring program for researchers interested in learning 
about the nuts and bolts of scholarly peer review in a dynamic, respectful, and global 
settings. Even though this program is reserach topic agnostic, it may have a bias towards 
life science fields.

Our goal is to support early-career researchers (*i.e.*, Master's level students and above 
in the academic track) by sharing aggregated knowledge about scholarly peer review, 
connecting them to peers and other stakeholders in the community,
and empowering them to become constructive members of the scientific community.

This program is part of an open project called [PREreview](https://content.prereview.org/about/) whose **mission** at is to bring more diversity to scholarly peer review by supporting and empowering community of researchers, particularly those at early stages of their career, to review preprints. We created a [free and open web platform](https://prereview.org) in which anyone with an ORCID iD can provide constructive feedback to preprints.

## Who are we?

First and foremost, we are a team of women scientists dedicated to making academia a diverse and inclusive space.

We are also advocate for open practices and are involved in several open commutities such as [ASAPbio Ambassadors](https://asapbio.org/asapbio-ambassadors), [Mozilla Open Leaders](https://foundation.mozilla.org/en/opportunity/mozilla-open-leaders/),
[eLIFE Ambassadors](https://elifesciences.org/inside-elife/a946c355/elife-community-ambassadors-243-volunteers-join-the-programme-in-2019), and [OpenCon](https://www.opencon2018.org/). 

## What do we need?

**You!** In whatever way you can help.

We need expertise in peer review (both traditional and innovative), diversity and inclusion, open-science, training, mentoring, leadership, communication, community building.

## Get involved

If you think you can help in any of the areas listed above (and we bet you can)
or in any of the many areas that we haven't yet thought of (and here we're sure
you can) then please check out [our contributors' guidelines](CONTRIBUTING.md)
and our [roadmap](roadmap.md).

Please note that it's very important to us that we maintain a positive and
supportive environment for everyone who wants to participate. When you join us
we ask that you follow our [code of conduct](CODE_OF_CONDUCT.md) in all
interactions both on and offline.

## How can I generate the website locally?

You need a `ruby` environment (version >= 2.4). Either you have it installed and
you know how to install [Bundler](https://bundler.io/) and
[Jekyll](https://jekyllrb.com/) and then run Jekyll, or you use
(mini-)[conda](https://conda.io/docs/index.html), a package management system
that can install all these tools for you. You can install it by following the
instructions on this page: https://conda.io/docs/user-guide/install/index.html

In the sequel, we assume you use miniconda.

1. Open a terminal
2. Clone this GitHub repository:

   ```
   git clone https://github.com/open-life-science/open-life-science.github.io.git
   ```

3. Navigate to the `open-life-science.github.io/` folder with `cd`
4. Set up the conda environment:

   ```
   make create-env
   ```

5. Install the project's dependencies:

   ```
   make install
   ```

6. Start the website:

   ```
   make serve
   ```

7. Open the website in your favorite browser at:
   [http://127.0.0.1:4000/](http://127.0.0.1:4000/)

## Run the link checks

To avoid dead or wrong links, run the link checkers:

```
make check-html
```

## Create a new blog post

To create a new blog post:

1. Create a file in the folder `_posts` with a file named following the pattern `yyyy-mm-dd-name.md`
2. Add some metadata on the top of the file

    ```
    ---
    layout: post
    title: <title of the post>
    author: <github id of the author>
    image: images/yyyy-mm-dd-name.jpg
    ---
    ```

4. Add content of the post in the file in Markdown
3. Add images in `images/posts/`

## Add someone as mentor, expert or organizer

1. Open the `_data/people.yaml` file
2. Create a new entry there (using the GitHub id) following the alphabetical order
3. Fill in information using the tags:
    - `name`
    - `email`
    - `website`
    - `twitter`
    - `gitter`
    - `orcid`
    - `description`
4. Add if the person should be listed as mentor by adding `mentor: true`
5. Add if the person should be listed as expert by adding `expert: true`
6. Add if the person should be listed as organizer by adding `organizer: true`
    
## Add a partner/sponsor

1. Open the `_data/partners.yaml` file
2. Create a new entry there (using the name in lowercase, with spaces replaced by `-`) following an alphabetical order
3. Fill in information using the tags:
    - `name`
    - `website`
    - `description`
4. Add a logo (if possible) named as the entry in `images/partners` folder
5. Add the path to the logo in `_data/partners.yaml` using `logo` tag
