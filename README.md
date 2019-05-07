# ![LOGO](logo.png) Remote Diagnostic Support **flow**ground Connector

## Description

A generated **flow**ground connector for the Remote Diagnostic Support API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/mercedes-benz.com/diagnostics/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:42:59+03:00

## API Description

The Remote Diagnostic Support API will provide the possibility for 3rd party applications (e.g. ADAC, ATU, etc.) to access vehicle diagnostics data remotely on behalf of the Daimler customer. To use the endpoints you need a valid vin/fin (vehicleId).

## Authorization

This API does not require authorization.

## Actions

### View the List of DTCs for specific vehicleId.

> This API creates a readout of DTCs for one vehicle. If the result is available immediately, the result is returned. If the result isn't available, a location to the DTC readout is returned. This location shall be polled until the result is available. INFO: GET Requests are not yet supported!

*Tags:* `Diagnostic Trouble Codes (DTC's)`

#### Input Parameters
* `vehicleId` - _required_ - The vehicle identifier of the vehicle to read from.
* `ecuId` - _optional_ - Return DTCs from this ECU id only. Default: Return DTCs from all ECUs.
* `dtcStatus` - _optional_ - Returns DTCs with this statuses only. Default: Return DTCs with all statuses.

### View the List of DTC Snapshot for specific vehicleId.

> This API creates a readout of a DTC snapshot from one vehicle. If the result is available immediately, the result is returned. If the result isn't available, a location to the DTC snapshot readout is returned. This location shall be polled until the result is available. INFO: GET Requests are not yet supported!

*Tags:* `Diagnostic Trouble Code (DTC) Snapshots`

#### Input Parameters
* `vehicleId` - _required_ - The vehicle identifier of the vehicle to read from
* `ecuId` - _required_ - The id of the ECU to read from
* `dtcId` - _required_ - The id of the DTC associated with the snapshot

### View the List of ECU for specific vehicleId.

> This API creates a readout of ECUs for one vehicle. If the result is available immediately, the result is returned. If the result isn't available, a location to the ECU readout is returned. This location shall be polled until the result is available. INFO: GET Requests are not yet supported!

*Tags:* `Electronical Control Units (ECU's)`

#### Input Parameters
* `vehicleId` - _required_ - The vehicle identifier of the vehicle to read from
* `ecuId` - _optional_ - Return this ECU id only. Default: Return all ECUs.

### View the List of resources

> This API creates a readout of available resources to the accessing party for one vehicle. If the result is available immediately, the result is returned. If the result isn't available, a location to the resource readout is returned. This location shall be polled until the result is available. INFO: GET Requests are not yet supported!

*Tags:* `Resources`

#### Input Parameters
* `vehicleId` - _required_ - vehicleId of the resources to be viewed

## License

**flow**ground :- Telekom iPaaS / mercedes-benz-com-diagnostics-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
