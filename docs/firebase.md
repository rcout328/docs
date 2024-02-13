# CRUD Operations Guide

## Create (C) - Add Data

### Capture Input:

In your "Add Data" component, capture user input using a state variable (data). Typically done using an input field and an onChange handler.

### Add Data to Firestore:

Create a reference to the Firestore collection where you want to store the data. Use `setDoc` to add the data to Firestore, providing the document reference and the data object.

### User Feedback:

Provide feedback to the user, indicating whether the data was added successfully or if there was an error.

## Read (R) - Fetch Data

### Fetch Data from Firestore:

In your "Read" component, create a reference to the Firestore collection. Use `getDocs` to retrieve a snapshot of the documents in the collection.

### Update State:

Update the component's state with the fetched data. Typically done by iterating over the snapshot and extracting relevant data.

### Display Data:

Display the fetched data in your component. In your case, you're mapping over the data to create a list of items.

## Update (U) - Update Data

### Select Data for Update:

When the user clicks the "Update" button, set the `selectedDocId` state with the ID of the document to be updated.

### Modify Data:

Allow the user to modify the data in an input field.

### Update Data in Firestore:

Create a reference to the specific document in Firestore using `doc`. Use `updateDoc` to update the data, providing the document reference and the modified data.

### Refresh Data:

After updating, refresh the displayed data by fetching it again from Firestore.

## Delete (D) - Delete Data

### Select Data for Delete:

When the user clicks the "Delete" button, set the `selectedDocId` state with the ID of the document to be deleted.

### Delete Data in Firestore:

Create a reference to the specific document in Firestore using `doc`. Use `deleteDoc` to delete the document, providing the document reference.

### Refresh Data:

After deletion, refresh the displayed data by fetching it again from Firestore.

### Reset States:

Reset any states related to the deleted or updated data, such as `selectedDocId` and `newData`.

#CRUD Operations Guide 📝
Create (C) - Add Data 🚀
Capture Input:
In your "Add Data" component, capture user input using a state variable (data). Typically done using an input field and an onChange handler.

Add Data to Firestore:
Create a reference to the Firestore collection where you want to store the data. Use setDoc to add the data to Firestore, providing the document reference and the data object.

User Feedback:
Provide feedback to the user, indicating whether the data was added successfully or if there was an error.

Read (R) - Fetch Data 📚
Fetch Data from Firestore:
In your "Read" component, create a reference to the Firestore collection. Use getDocs to retrieve a snapshot of the documents in the collection.

Update State:
Update the component's state with the fetched data. Typically done by iterating over the snapshot and extracting relevant data.

Display Data:
Display the fetched data in your component. In your case, you're mapping over the data to create a list of items.

Update (U) - Update Data 🔄
Select Data for Update:
When the user clicks the "Update" button, set the selectedDocId state with the ID of the document to be updated.

Modify Data:
Allow the user to modify the data in an input field.

Update Data in Firestore:
Create a reference to the specific document in Firestore using doc. Use updateDoc to update the data, providing the document reference and the modified data.

Refresh Data:
After updating, refresh the displayed data by fetching it again from Firestore.

Delete (D) - Delete Data 🗑️
Select Data for Delete:
When the user clicks the "Delete" button, set the selectedDocId state with the ID of the document to be deleted.

Delete Data in Firestore:
Create a reference to the specific document in Firestore using doc. Use deleteDoc to delete the document, providing the document reference.

Refresh Data:
After deletion, refresh the displayed data by fetching it again from Firestore.

Reset States:
Reset any states related to the deleted or updated data, such as selectedDocId and newData.
