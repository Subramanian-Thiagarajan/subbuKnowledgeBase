#### Need for file formats
- Store and process large datasets
- Continuously evolving schema
- Cost effectiveness
- Transit data

#### Considerations for choosing file formats
- Row/Columnar
- Read/Write Heavy
- Splittable Data
- Schema evolution support
- Compression support

## File Formats

#### CSV 
- Tabular Data, Row Based
- Fast Write / Slow Read
- Splittable
- Schema Evolution Support Limited
- Compression Support Limited

#### JSON 
- Key Value Pairs, NoSQL DB 
- Slow R/W
- Not splittable (lacks indexing)
- Compression Easy
- Supports SES 

#### Parquet
- Columnar format
- Only required columns retrieved - Reduces Disk/IO - Projection Pushdown
- Binary files with metadata
- Heavy R/W possible
- SES, CS Supported
- Splittable

#### AVRO 
- Row Based
- Highly Splittable - Due to sync markers for blocks
- Binary format
- SES Robust support
- Write Heavy

#### ORC 
- Row Columnar format
- Row Data in Columnar format
- Splittable without markers
- SES, CS support
- R/W heavy