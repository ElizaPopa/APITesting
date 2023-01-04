# APITesting

Below some test cases I made for APIs + screenshots from Postman

----------------------------

**Description:** Open an API on Postman website

** Steps to Reproduce:** 

1. Go to https://speeding-meadow-227188.postman.co
2. Log in with your credentials
3. Click on "Workspaces"
4. Click on "My Workspace"
5. Hit the "New" button 
6. Select "HTTP" request

**Expected results:** A new API is open to be created/updated/deleted

**Environment:** Safari

----------------------------

**Description:** Create an API/ Add a new pet to the store (using Swagger website)

**Preconditions:** Open the Postman website version: https://speeding-meadow-227188.postman.co & log in with your credentials

**STR:** 

1. Click on "Workspaces", then ""My Workspace"
2. Hit the "New" button 
3. Select "HTTP" request
4. Select "POST" from droplist
5. Copy base URL from Swagger website "petstore.swagger.io/v2"
6. Insert "https://" + paste "petstore.swagger.io/v2" in URL textbox
7. Add "/pet" after the new created URL "https://petstore.swagger.io/v2"
8. Click on "Body"
9. Select "raw" option
10. Select "JSON" from the blue droplist
11. Go to https://petstore.swagger.io/#/pet/addPet
12. Click on the second "POST" button from the pet section
13. Copy required body object from the black textbox
14. Paste on Postman the copied text in cell 1
15. Complete the textbox with details: id, name, status for the new pet
16. Hit the "Send" button

**Expected results:** The new pet has been successfully added with Status: 200 OK and all the details are displayed in the Body textbox.

**Test data:** id: 1 & name: "Alfie"

**Environment:** Safari

![Add a new pet : API](https://user-images.githubusercontent.com/109477059/210549721-4c0da3dc-aaca-4518-a20b-ff8dd508b1f8.png)

-------------------------------

**Description:** Update an existing pet

**Preconditions:** Open the Postman website version: https://speeding-meadow-227188.postman.co & log in with your credentials

**Steps to Reproduce:** 

1. Open a new API: Workspaces/My Workspaces/ New/ Select "HTTP" request
2. Select "PUT" from droplist
3. Add https://petstore.swagger.io/v2/pet into requested URL textbox
4. Go to https://petstore.swagger.io/#/pet/updatePet and copy the required body
5. Paste it on Postman in Body/raw/json/cell 1
6. Update "id" with "7" and "name" with "Max"
7. Hit the "Send" button

**Expected results:** The new pet has been successfully updated and all the details are displayed into the Body textbox

**Environment:** Safari
