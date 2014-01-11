# friskis.py

### What is it?
A simple scraper for the Friskis & Svettis Linköping website. Right now, it provides helpers for logging in, fetching all available shifts, and book shifts.

### How can I use it?
    from friskis import FriskisClient

    client = FriskisClient()
    client.login(username='bob', password='passw0rd')

    for shift in client.get_available_shifts():
        print shift

    shift[0].book(client.session)


### Does it have feature X?
Probably not.

### Does it handle special case Y?
Most certainly not. At least not yet.
