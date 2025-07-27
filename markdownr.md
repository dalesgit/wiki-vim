---
title: markdownr
date: 2024-07-17
tags: 
---
# markdownr
# sanzoghenzo/markdownr: Android app that converts an URL to markdown, and lets you share it to your favorite notes app.

Android app that converts an URL to markdown, and lets you share it to your favorite notes app.

I've written this app to save articles I found interesting to a note taking app that uses markdown and git to sync notes to my pc.

[![Get it on F-Droid](https://camo.githubusercontent.com/f422f6f830e814ec7e766de8fef4db949c6add75a9d58548ab2f5d29855c0616/68747470733a2f2f6664726f69642e6769746c61622e696f2f617274776f726b2f62616467652f6765742d69742d6f6e2e706e67)](https://f-droid.org/packages/com.sanzoghenzo.markdownr/)

[![markdownr-from-intent-small](https://private-user-images.githubusercontent.com/977953/282924291-091d07a1-f917-4a57-b70c-72f9aa088c6e.gif?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjEyMjMzMDksIm5iZiI6MTcyMTIyMzAwOSwicGF0aCI6Ii85Nzc5NTMvMjgyOTI0MjkxLTA5MWQwN2ExLWY5MTctNGE1Ny1iNzBjLTcyZjlhYTA4OGM2ZS5naWY_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcxN1QxMzMwMDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT02YzE2M2FmMDBiODM3ZmE3ODBlYTNiY2I2NWE0YWQ0MTFmMzJhMTNhNTVlZTkxMGNiNDJmNmRjYzBhODA3NjUzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.idC5-fEOuFABP4nM8iCEAbfLURkIsu8tYcbQzAhv6dQ)](https://private-user-images.githubusercontent.com/977953/282924291-091d07a1-f917-4a57-b70c-72f9aa088c6e.gif?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjEyMjMzMDksIm5iZiI6MTcyMTIyMzAwOSwicGF0aCI6Ii85Nzc5NTMvMjgyOTI0MjkxLTA5MWQwN2ExLWY5MTctNGE1Ny1iNzBjLTcyZjlhYTA4OGM2ZS5naWY_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcxN1QxMzMwMDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT02YzE2M2FmMDBiODM3ZmE3ODBlYTNiY2I2NWE0YWQ0MTFmMzJhMTNhNTVlZTkxMGNiNDJmNmRjYzBhODA3NjUzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.idC5-fEOuFABP4nM8iCEAbfLURkIsu8tYcbQzAhv6dQ)[![markdownr-options-small](https://private-user-images.githubusercontent.com/977953/282924332-6108ab52-540c-4c41-9889-8b59244eee3b.gif?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjEyMjMzMDksIm5iZiI6MTcyMTIyMzAwOSwicGF0aCI6Ii85Nzc5NTMvMjgyOTI0MzMyLTYxMDhhYjUyLTU0MGMtNGM0MS05ODg5LThiNTkyNDRlZWUzYi5naWY_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcxN1QxMzMwMDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT05YTc5NTJmMDBmNTdlODczNmI0N2U2ZDM0NjIwOTBjYjhjZDRiMDZkMWQ1MGRhYzAzNWZiZjBjMTFkOTlhOGE5JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.RJulAv0IRHeGhHeGGTtzvHqafzOaqU_HmmDE2H1n65U)](https://private-user-images.githubusercontent.com/977953/282924332-6108ab52-540c-4c41-9889-8b59244eee3b.gif?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjEyMjMzMDksIm5iZiI6MTcyMTIyMzAwOSwicGF0aCI6Ii85Nzc5NTMvMjgyOTI0MzMyLTYxMDhhYjUyLTU0MGMtNGM0MS05ODg5LThiNTkyNDRlZWUzYi5naWY_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcxN1QxMzMwMDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT05YTc5NTJmMDBmNTdlODczNmI0N2U2ZDM0NjIwOTBjYjhjZDRiMDZkMWQ1MGRhYzAzNWZiZjBjMTFkOTlhOGE5JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.RJulAv0IRHeGhHeGGTtzvHqafzOaqU_HmmDE2H1n65U)

-   Downloads the web page specified in the URL input field, cleans it up (like readability does) and converts it to Markdown.
-   Ability to enable/disable parts of the markdown:
    -   YAML front matter with the creation date, the source url and the author
    -   The "Clipped from " text under the title
    -   The excerpt of the article
    -   The article body
-   Ability to show the markdown preview
-   Share the markdown to other apps with standard share intent.
-   The URL can be also be shared from another app (for example the web browser); markdownr will automatically convert it and show the share intent.
-   If something isn't working with the share button, you can use the copy button to send the text to the clipboard.

This app has been made possible thanks ti these wonderful libraries:

-   `html2md`
-   `readability4J`
-   `receive\_sharing\_intent`
-   `share_plus`
-   `flutter_markdown`
-   `http`
-   `shared_preferences`
-   `fluttertoast`
-   `intl`
-   `flutter\_charset\_detector`
-   `charset_converter`

I just put them together in a really simple app.
