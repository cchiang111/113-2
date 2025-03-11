library(tidyverse)

# Ensure correct variable types
reshaped_travel_data <- reshaped_travel_data %>%
  mutate(
    首站抵達地 = as.factor(首站抵達地),
    細分 = as.factor(細分),
    Year = as.integer(Year),
    Number_of_Travelers = as.integer(Number_of_Travelers)
  )

# Verify structure
str(reshaped_travel_data)
