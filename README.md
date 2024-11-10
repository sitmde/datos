# Migratory flow of Colombians

This dataset provides information on migration flows from 2012 to 2024.

| Column Name               | Description                                                                                                                     | Type |
|---------------------------|---------------------------------------------------------------------------------------------------------------------------------|------|
| cantidad_de_filas         | Total number of migration flow records.                                                                                        |   integer |
| agnio                     | The year of the records.                                                                                                        |  string |
| region_destino            | Region to which travelers are heading (entry region or destination region for exit).                                           |   string |
| region_nacionalidad       | Region of the traveler's nationality.                                                                                           |  string |
| entrada_salida            | Indicates if travelers are arriving in or departing from Colombia.                                                             |  string |
| sexo                      | Gender: F (Female), M (Male), I (Indeterminate).                                                                                |  string |
| categoria_migratoria      | Permits granted for entry into Colombia - PT, POA, PID, types of visas (resident, etc.), as per Resolution 3167 of 2019.       |  string |
| motivo_viaje              | Activity authorized to be undertaken in the country.                                                                           |  string |
| departamento_hospedaje    | Only applies to foreigners entering Colombia.                                                                                  |  string |
| ciudad_hospedaje          | Only applies to foreigners entering Colombia.                                                                                  |  string | 
| colombiano_extranjero     | Indicates if the person is Colombian or a foreigner.                                                                           |  string |
| puesto_migratorio         | The checkpoint where the migration flow was recorded.                                                                          |  string |
| tipo_transporte           | Type of transport used by the traveler ('Air', 'Land', 'Sea', 'River'). "Unauthorized" indicates visa regularization via trochas, starting from 2014. |  string |
| centro_regional           | Migration flows (entries and exits) managed by the regional center.                                                            |  string |
| pais_nacionalidad         | Nationality of the traveler.                                                                                                   |  string |
| meses                     | Month in which the migration flow occurred.                                                                                    |  string |
| pais_destino_procedencia  | Country to which the traveler is heading.                                                                                      |  string |
| rango_edad                | Generated based on the date of birth versus the date of the migration flow.                                                    |  string |
| departamento              | Department where the Migration Control Post (PCM) is located.                                                                  |  string |



# National Tourism Registry - RNT

Public registry in which all tourism service providers operating within the territory of Colombia must register.

| Column Name                       | Description                                                                                                  | Data Type   |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------|-------------|
| ano                                | Year corresponding to the national tourism registry                                                         | Number      |
| mes                                | Month number corresponding to the National Tourism Registry                                                 | Number      |
| codigo_rnt                         | National Tourism Registry number                                                                            | Number      |
| cod_mun                            | Divipola code for the municipality established by DANE                                                      | Number      |
| cod_dpto                           | Divipola code for the department established by DANE                                                        | Number      |
| estado_rnt                         | Current status of the establishment's National Tourism Registry                                             | Text        |
| razon_social_establecimiento       | Name of the establishment                                                                                   | Text        |
| departamento                       | Name of the department in Colombia                                                                          | Text        |
| municipio                          | Name of the municipality in Colombia                                                                        | Text        |
| categoria                          | General description of tourism activities, e.g., travel agency, lodging establishment, etc.                 | Text        |
| sub_categoria                      | Specific tourism activities within the general category, e.g., travel agency, hotel, apart-hotel, etc.      | Text        |
| habitaciones                       | Number of rooms available (if applicable)                                                                   | Number      |
| camas                              | Total number of beds available (if applicable)                                                              | Number      |
| num_emp1                            | Total number of employees in the establishment (if applicable)                                             | Number      |
| correo_establecimiento             | Establishment's email address                                                                               | Text        |


# HSI 

Source SIT, Mabrian data

| # | Column       | Description | Non-Null Count | Dtype   |
|---|--------------| ------------|----------------|---------|
| 0 | destination  | Medellín       | 80 non-null    | object  |
| 1 | origin       | Country origin | 53 non-null    | object  |
| 2 | hotel_id     | hotel identifier | 80 non-null    | object  |
| 3 | start_date   | Reported month | 80 non-null    | object  |
| 4 | hsi          | Hotel satisfaction index  | 80 non-null    | float64 |

**Summary**
- **Entries**: 80
- **Total Columns**: 5
- **Data Types**: 4 object, 1 float64
- **Memory Usage**: 3.2+ KB


# HOTELS 

This `DataFrame` contains information on 215 hotels, with a total of 7 columns. Below is a description of each variable in the dataset.

| # | Variable              | Type     | Non-Null Count | Description |
|---|-----------------------|----------|----------------|-------------|
| 0 | `sustainability_level` | object   | 88            | The sustainability level of the hotel. Indicates the hotel's commitment to sustainable practices. May be categorized into levels or categories and contains missing values for hotels without sustainability information. |
| 1 | `hotel_groupings`      | object   | 215           | Hotel groupings. This variable classifies hotels into different groups, possibly based on shared characteristics or location. All entries have a value in this column. |
| 2 | `name`                 | object   | 215           | The name of the hotel. The unique identifier or commercial name of each hotel in the dataset. No missing values. |
| 3 | `stars`                | int64    | 215           | The hotel's star rating (integer). Indicates the category or quality of the hotel, usually on a scale from 1 to 5. No missing values. |
| 4 | `latitude`             | float64  | 213           | The latitude of the hotel. Geographic coordinate indicating the hotel's position in terms of latitude. Two records contain missing values. |
| 5 | `longitude`            | float64  | 213           | The longitude of the hotel. Geographic coordinate indicating the hotel's position in terms of longitude. Two records contain missing values. |
| 6 | `id`                   | object   | 215           | Unique identifier for each hotel. This is a unique identifier in text format for each hotel. No missing values. |

## DataFrame Summary

- **Total Entries**: 215
- **Total Columns**: 7
- **Data Types**: 
  - 4 columns of type `object`
  - 1 column of type `int64`
  - 2 columns of type `float64`
- **Memory Usage**: 11.9 KB

This dataset allows for analysis of geographic location, star ratings, sustainability levels, and other hotel characteristics. The coordinate columns (`latitude` and `longitude`) are useful for spatial analyses or map visualizations.
