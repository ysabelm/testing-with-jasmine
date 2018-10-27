# JavaScript Testing

Practice testing your javascript applications using Jasmine library.

## First step
`git clone https://github.com/udacity/ud549` and open the files in your editor to follow along with [Udacity's JavaScript Testing course](https://www.udacity.com/course/javascript-testing--ud549).

## Test Address Book functionalities
describe ('name', function) {
    it('...')

    it('...')
}
`ìt` is used to identify a specification, or a spec, which is just a container for a test, a way to identify the exact tested feature. `ìt` is like a boundary. `describe`is used to identify a suite, a group of related specs. For this example, the name = AddressBook, we test all that is related to the address book.

### Test add and get contact features in an address book
Using Red-Green-Refactoring method, test the "add contact" feature. First, we have to write the test in spec/AddressBookSpec.js and check it fails using Jasmine Spec Runner (Red). `AddressBook is not defined`. To let it pass, we have to write a constructor function - function AddressBook() - While refreshing, we read `Contact is not defined` --> We also need to write a contact constructor in a new file and add it as a src file in the html file...and so on. Neither addContact or getContact are defined --> we need to write them.

### Test delete feature in an address book
In spec/AddressBook.js, we write the test and check it also fails using Jasmine Spec Runner. writing the spec, I expect the object `not.toBeDefined` if I try to get it from the address book. We need to write in AddressBook.js the delete function using the splice method of an array to remove a contact.

### Removing redundant code
Instead of setting up the AddressBook and the Contact in each of our specs, we can use a function that should be run before each of the tests : it's the `beforeEach` function.


## Dependencies
[Jasmine](https://jasmine.github.io/pages/getting_started.html)
Included is a sample app and sample tests. Open SpecRunner.html and run the included specs. Both the source files and their respective specs are linked in the <head> of the SpecRunner.html. To start using Jasmine, replace the source/spec files with your own.
Load the SpecRunner.html in your favorite browser.


