# R Script for Days Since Counter

# Function to calculate the number of days since a given date
days_since <- function(start_date) {
  start <- as.Date(start_date)
  today <- Sys.Date()
  days <- as.numeric(today - start)
  return(days)
}

# Set your chosen start date here
chosen_start_date <- "2024-11-23"

# Calculate days since the chosen date
counter <- days_since(chosen_start_date)

# Print the result
cat("Days since", chosen_start_date, ":", counter, "days\n")
