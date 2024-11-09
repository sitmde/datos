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
