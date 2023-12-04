# Unit2.PartyPlanner

# Unit2.PartyPlanner

A user enters the website and finds a list of the names, dates, times, locations, and descriptions of all the parties that are happening.
Next to each party in the list is a delete button. The user clicks the delete button for one of the parties. That party is then removed from the list.
There is also a form that allows the user to enter information about a new party that they want to schedule. After filling out the form and submitting it, the user observes their party added to the list of parties.



{
    success: true, // or false
    error: {
      name: "ErrorName",
      message: "This is an error message."
    }, // or null
    data: {
      example: "This is some data."
    }, // or null
  }


{
    id: 1,
    name: "Recipe Name",
    imageUrl: "https://www.example.com/image.jpg",
    description: "This is a description of the recipe."
  }

{
    id: 1,
    name: "Artist Name",
    imageUrl: "https://www.example.com/image.jpg",
    description: "This is a description of the artist."
  }

{
    id: 1,
    name: "Event Name",
    description: "This is a description of the event.",
    date: "2021-09-30T00:00:00.000Z", // Date ISO string
    location: "123 Street"
  }

{
    id: 1,
    name: "Guest Name",
    email: "guest@email.com",
    phone: "123-456-7890"
  }

{
    id: 1,
    guestId: 1, // Id of the attending guest
    eventId: 1  // Id of the event being attended
  }      


Each resource has the following endpoints:

GET /<resource>
Sends an array of objects for the requested resource.

GET /<resource>/<id>
Sends a single object identified by the given id.

POST /<resource>
Attempts to create a new object. If successful, the created object is returned.

PUT /<resource>/<id>
Attempts to update the object identified by the given id. If successful, the updated object is returned.

DELETE /<resource>/<id>
Attempts to delete the object identified by the given id. Sends status code 204 if successful.
