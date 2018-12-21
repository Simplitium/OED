# Changes to OED DB

## OED v1.0.1:

•	Updates to data types:

  o	Smallint to float (previously too restrictive, needed a data type that accepts decimals): FirstFloorHeight, GroundElevation,    BaseFloodElevation, BuildingHeight, FloodDefenseHeight in LocationDetails table
  
•	Allows NULLs (previously too restrict):

  o	Locations table:
  
    -	LocInceptionDate
    -	LocExpiryDate
    -	CompletionDate
    
  o	Policies table:
  
    -	InceptionDate
    -	ExpiryDate
    
  o	ReinsuranceInfo table:
  
    -	ReinsInceptionDate
    -	ReinsExpiryDate
    
•	Default values removed from:

  o	Locations table (redundant default):
  
    -	CompletionDate
    -	BuildingTIV
    -	OtherTIV
    -	ContentsTIV
    -	BITIV
    
  o	ReinsuranceInfo table (requesting the field to always be populated by the user, making default redundant):
  
    -	PlacedPercent

•	Default values added to:

  o	Portfolios table – added getdate():
  
    -	CreatedOn
    -	EditedOn

•	Fields renamed:

  o	NumberOfStories to NumberOfStoreys in Locations table.

•	New tables:

  o	xFXRateFiles – a table to store different currency exchange rate files by user

•	New Fields:

  o	FileID in xFXRates tables

## Reference table updates:
•	xRiskLevel table updated to accept blanks. SEL is no longer available as one of the acceptable values. The same is achieved by using blank.

## Bugs fixed:
•	Autoincrement removed from LocationDetails.LocID.
