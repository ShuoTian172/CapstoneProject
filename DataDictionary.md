# DEND Capstone

# **Data Dictionary Dimension Tables**
## new_airport_data
 * i94_port: string (nullable = false)
 * i94_airport_name: string (nullable = false)
 * i94_airport_state: string (nullable = false)

 
## country_codes_iso_df_spark
 * country_code: string (nullable = false)
 * country_name: string (nullable = false
 * alpha_2: string (nullable = false)
 * alpha_3: string (nullable = false)
 * iso_3166_2: string (nullable = false)
 * region: string (nullable = true)
 * sub_region: string (nullable = true)
 * intermediate_region: string (nullable = false)
 * region_code: string (nullable = true)
 * sub_region_code: string (nullable = true)
 * intermediate_region_code: string (nullable = false)
 
## new_I94_Data
 * cicid: double (nullable = true)-ID number of each individual
 * year: integer (nullable = true)-Year of Immigration
 * month: integer (nullable = true)-Month of Immigration
 * i94port: string (nullable = true)-City Port Code where Immigrant entered
 
## new_Temperatures_joined
 * year: integer (nullable = true)-Temperature Year
 * month: integer (nullable = true)-Temerpature Month
 * avg_temp_celcius: double (nullable = true)-Avg Temperature in Celcius
 * avg_temp_fahrenheit: double (nullable = true)-Avg Temperatrue in Fahrenheit
 * Country: string (nullable = true)- Country name
 * i94_cit: integer (nullable = true)
 * i94_country_name: string (nullable = false)
 * iso_country_code: string (nullable = false)


# Fact Table(immigrations_table)
 * cicid: double (nullable = true)-ID number of each individual
 * avg_temp_fahrenheit: double (nullable = true)-Avg Temperature in Celcius
 * airport_id: string (nullable = true)
 * country_id: integer (nullable = true)
 * country_name: string (nullable = false)


