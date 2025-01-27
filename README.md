
# The JETSCAPE Organization Website

This repository hosts the JETSCAPE Organization Website.

The site is 
automatically updated and deployed through GitHub Actions when changes are 
pushed (or pull requests are merged) to the main branch.

The site is live at https://jetscape.github.io and is also reachable at our https://jetscape.org domain.

---
JSON files in the [/data](/data) folder are used to populate lists and tables throughout the site.  To update those lists and tables, update the corresponding JSON file.

* [/data/jetscapeMeetings.json](/data/jetscapeMeetings.json) provides the data for the **JETSCAPE Meetings** table on the [Meetings](/meetings.html) page.

* [/data/otherMeetings.json](/data/otherMeetings.json) provides the data for the **Other Meetings of Interest** table on the [Meetings](/meetings.html) page.

* [/data/publications.json](/data/publications.json) provides the data for the **Publications** list on the [Publications](/publications.html) page.

* [/data/talks.json](/data/talks.json) provides the data for the **Talks** table on the [Talks](/talks.html) page.

* [/data/JETSCAPE_Authors.json](/data/JETSCAPE_Authors.json) is built automatically from [/data/JETSCAPE_Authors.csv](/data/JETSCAPE_Authors.csv) and populates the author names and affiliations on the [Members](/members.html) page.  To update the members, update the .csv file.  A [GitHub Actions workflow](/.github/workflows/parseCSV.yaml) runs on pushes and pull requests to the **main** branch to generate the corresponding .json file.  Updates to the .csv must maintain the same document structure and delimiters as read by [/scripts/parseAuthors.py](/scripts/parseAuthors.py).

## Requesting Site Updates

Since the site is now managed as a GitHub repository, JETSCAPE collaborators are welcome to create issues [here](https://github.com/JETSCAPE/JETSCAPE.github.io/issues) and submit pull requests [here](https://github.com/JETSCAPE/JETSCAPE.github.io/pulls).
