
def display_menu():
    print("\nContact Book Menu:")
    print("1. Add a new contact")
    print("2. Update an existing contact")
    print("3. View all contacts")
    print("4. Exit")

def add_contact(contact_book):
    name = input("Enter contact name: ")
    if name in contact_book:
        print("This contact already exists. Please update it if you need to.")
        return
    phone = input("Enter phone number: ")
    email = input("Enter email address: ")
    contact_book[name] = {'Phone': phone, 'Email': email}
    print(f"Contact {name} added successfully!")

def update_contact(contact_book):
    name = input("Enter the contact name to update: ")
    if name not in contact_book:
        print("Contact not found.")
        return
    phone = input("Enter new phone number: ")
    email = input("Enter new email address: ")
    contact_book[name] = {'Phone': phone, 'Email': email}
    print(f"Contact {name} updated successfully!")

def view_contacts(contact_book):
    if not contact_book:
        print("No contacts found.")
        return
    print("\n--- Contact List ---")
    for name, details in contact_book.items():
        print(f"Name: {name}, Phone: {details['Phone']}, Email: {details['Email']}")
    print("--------------------")

def main():
    contact_book = {}
    
    while True:
        display_menu()
        choice = input("Enter your choice (1-4): ")
        
        if choice == '1':
            add_contact(contact_book)
        elif choice == '2':
            update_contact(contact_book)
        elif choice == '3':
            view_contacts(contact_book)
        elif choice == '4':
            print("Exiting the Contact Book. Goodbye!")
            break
        else:
            print("Invalid choice. Please select a valid option.")

if __name__ == "__main__":
    main()










