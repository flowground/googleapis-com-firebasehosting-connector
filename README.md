# ![LOGO](logo.png) Firebase Hosting **flow**ground Connector

## Description

A generated **flow**ground connector for the Firebase Hosting API (version v1beta1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/firebasehosting/v1beta1/swagger.json<br/>
Generated at: 2019-05-07T17:41:38+03:00

## API Description

The Firebase Hosting REST API enables programmatic and customizable deployments to your Firebase-hosted sites. Use this REST API to deploy new or updated hosting configurations and content files.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Deletes the existing domain mapping on the specified site.

*Tags:* `sites`

#### Input Parameters
* `name` - _required_ - Required. The name of the domain association to delete.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Gets a domain mapping on the specified site.

*Tags:* `sites`

#### Input Parameters
* `name` - _required_ - Required. The name of the domain configuration to get.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Updates the specified metadata for a version. Note that this method will<br/>
> fail with `FAILED_PRECONDITION` in the event of an invalid state<br/>
> transition. The only valid transition for a version is currently from a<br/>
> `CREATED` status to a `FINALIZED` status.<br/>
> Use [`DeleteVersion`](../sites.versions/delete) to set the status of a<br/>
> version to `DELETED`.

*Tags:* `sites`

#### Input Parameters
* `name` - _required_ - The unique identifier for a version, in the format:
<code>sites/<var>site-name</var>/versions/<var>versionID</var></code>
This name is provided in the response body when you call the
[`CreateVersion`](../sites.versions/create) endpoint.
* `updateMask` - _optional_ - A set of field names from your [version](../sites.versions) that you want
to update.
<br>A field will be overwritten if, and only if, it's in the mask.
<br>If a mask is not provided then a default mask of only
[`status`](../sites.versions#Version.FIELDS.status) will be used.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Updates the specified domain mapping, creating the mapping as if it does<br/>
> not exist.

*Tags:* `sites`

#### Input Parameters
* `name` - _required_ - Required. The name of the domain association to update or create, if an
association doesn't already exist.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists the domains for the specified site.

*Tags:* `sites`

#### Input Parameters
* `pageSize` - _optional_ - The page size to return. Defaults to 50.
* `pageToken` - _optional_ - The next_page_token from a previous request, if provided.
* `parent` - _required_ - Required. The parent for which to list domains, in the format:
<code>sites/<var>site-name</var></code>
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a domain mapping on the specified site.

*Tags:* `sites`

#### Input Parameters
* `parent` - _required_ - Required. The parent to create the domain association for, in the format:
<code>sites/<var>site-name</var></code>
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists the remaining files to be uploaded for the specified version.

*Tags:* `sites`

#### Input Parameters
* `pageSize` - _optional_ - The page size to return. Defaults to 1000.
* `pageToken` - _optional_ - The next_page_token from a previous request, if provided. This will be the
encoded version of a firebase.hosting.proto.metadata.ListFilesPageToken.
* `parent` - _required_ - Required. The parent to list files for, in the format:
<code>sites/<var>site-name</var>/versions/<var>versionID</var></code>
* `status` - _optional_ - The type of files in the version that should be listed.
    Possible values: STATUS_UNSPECIFIED, EXPECTED, ACTIVE.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists the releases that have been created on the specified site.

*Tags:* `sites`

#### Input Parameters
* `pageSize` - _optional_ - The page size to return. Defaults to 100.
* `pageToken` - _optional_ - The next_page_token from a previous request, if provided.
* `parent` - _required_ - Required. The parent for which to list files, in the format:
<code>sites/<var>site-name</var></code>
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a new release which makes the content of the specified version<br/>
> actively display on the site.

*Tags:* `sites`

#### Input Parameters
* `parent` - _required_ - The site that the release belongs to, in the format:
<code>sites/<var>site-name</var></code>
* `versionName` - _optional_ - The unique identifier for a version, in the format:
<code>/sites/<var>site-name</var>/versions/<var>versionID</var></code>
The <var>site-name</var> in this version identifier must match the
<var>site-name</var> in the `parent` parameter.
<br>
<br>This query parameter must be empty if the `type` field in the
request body is `SITE_DISABLE`.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a new version for a site.

*Tags:* `sites`

#### Input Parameters
* `parent` - _required_ - Required. The parent to create the version for, in the format:
<code>sites/<var>site-name</var></code>
* `sizeBytes` - _optional_ - The self-reported size of the version. This value is used for a pre-emptive
quota check for legacy version uploads.
* `versionId` - _optional_ - A unique id for the new version. This is only specified for legacy version
creations.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Adds content files to a version.

*Tags:* `sites`

#### Input Parameters
* `parent` - _required_ - Required. The version to add files to, in the format:
<code>sites/<var>site-name</var>/versions/<var>versionID</var></code>
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-firebasehosting-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
