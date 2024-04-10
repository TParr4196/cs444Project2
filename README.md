# Reservations

## Building
`make` to build. An executable called `reservations` will be produced.
`rm -f reservations` to clean up executable

## Files
`reservations.c`: Project 2 of cs444 designed to continue exploration of pthread library 
    through importance of mutex locks

## Data
Uses an array of booleans to keep track of whether an individual seat is free or in use

## Functions
`main`
    `seat_broker`: randomly reserves or frees a random seat transaction_count number of times
        `reserve_seat`: reserves a seat and updates seat count or returns that seat is taken
        `free_seat`: frees a seat and updates seat count or returns that seat is free
        `verify_seat_count`: traverses the array and counts number of taken seats. verifys against seat_taken_count

`is_free`: checks if a given seat is free

## Notes