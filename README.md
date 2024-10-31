This code implements an assistant for managing contact information and birthday reminders.

Classes:

- `Field` — base class for creating contact fields, including `Name`, `Phone`, and `Birthday`.
- `Name` — subclass of `Field` representing a contact's name.
- `Phone` — subclass of `Field` representing a phone number, with format validation.
- `Birthday` — subclass of `Field` storing a birthday date in the `DD.MM.YYYY` format.
- `Record` — stores contact information (name, phones, birthday) and allows phone editing.
- `AddressBook` — a dictionary of contacts with support for adding, deleting, searching, and retrieving birthday reminders.

Decorator:

- `input_error` — handles exceptions raised during command execution.

Main functions:

- `parse_input` — parses the user input into a command and arguments.
- `add_contact`, `change_number`, `show_phones`, `show_all`, `add_birthday`, `show_birthday`, `show_reminder` — user command handlers.
- `save_data`, `load_data` — functions for serializing and deserializing the address book data.
