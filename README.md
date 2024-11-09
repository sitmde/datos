# Flujo migratorio de Colombianos

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



