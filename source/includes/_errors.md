# Errors

<!-- <aside class="notice">
This error section is stored in a separate file in <code>includes/_errors.md</code>. Slate allows you to optionally separate out your docs into many files...just save them to the <code>includes</code> folder and add them to the top of your <code>index.md</code>'s frontmatter. Files are included in the order listed.
</aside> -->

The **Dine On Campus**&reg; API uses the following error codes:


| Error Code | Meaning                                                                                        |
| ---------- | ---------------------------------------------------------------------------------------------- |
| 400        | Bad Request -- Invalid request.                                                                |
| 401        | Unauthorized -- Invalid API key.                                                               |
| 403        | Forbidden -- Unauthorized request.                                                             |
| 404        | Not Found -- Invalid endpoint.                                                                 |
| 405        | Method Not Allowed -- Invalid method.                                                          |
| 406        | Not Acceptable -- Invalid format.                                                              |
| 410        | Gone -- Endpoint no longer exists.                                                             |
| 429        | Too Many Requests -- Request threshold exceeded.                                               |
| 500        | Internal Server Error -- Unexpected server error. Please try again later.                      |
| 503        | Service Unavailable -- Offline. Maintenance or possible network error. Please try again later. |
