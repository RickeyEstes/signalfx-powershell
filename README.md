# SignalFx-PowerShell

_This is a PowerShell wrapper around the SignalFx API._

## Usage

### API Tokens

The _cmdlets_ have an `ApiToken` parameter or the client will try to load tokens from `Env:\`.
The client will loads the appropriate token necessary for the _cmdlet_ from the environment if it's defined.

* **Org tokens - aka Access Tokens**
  * `SFX_ACCESS_TOKEN`
* **Session tokens - aka User API Access Tokens**
  * `SFX_USER_TOKEN`

SignalFx [documentation](https://developers.signalfx.com/basics/authentication.html) on API Authentication.

### Cmdlets

* **Get-SFxDimensionMetadata** - Retrieves metadata objects for which the metrics name matches the search criteria.
* **Publish-SFxEvent** - Sends custom events to SignalFx.
