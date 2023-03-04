# Photography Portfolio

This Vue application boasts a sleek frontend interface that offers users an array of features to manage their photo collection with ease. From viewing to creating, deleting, and updating photos, users have complete control over their media library. The application prioritizes user security by requiring authorization to access and manipulate photo data. Its intuitive interface design ensures effortless navigation, empowering users to efficiently manage their favorite photos. What's more, the app integrates with a robust backend service to guarantee secure storage and retrieval of event data.

Technologies Used
- Vue
- Javascript
- CSS
- HTML


## Component Architecture

```mermaid
flowchart TD

    App --> Header
    App --> Outlet
    App --> Footer
    Header --> Nav
    Nav --> id1[Home Link]
    Nav --> id2[Contact Link]
    Nav --> id3[Login Link]
    Outlet --> id4["/"] --> Index
    Outlet --> id5["/photos/:id"] --> Show
    Outlet --> id6["/create"] --> photoCreateAction
    Outlet --> id7["/update/:id"] --> photoUpdateAction
    Outlet --> id8["/delete/:id"] --> photoDeleteAction
```


## Frontend Route Table
|    Route    | Element |    Loader   |       Action      |              Description                     |
|-------------|---------|-------------|-------------------|----------------------------------------------|
|      /      |  Index  | indexLoader |                   | Loads up list of photos                      |
| /photo/:id  |  Show   | photoLoader |                   | Loads up a specific photo                    |
|   /create   |  Create |             | photoCreateAction | Handles submission of create form for photos |
| /update/:id |  Update |             | photoUpdateAction | Handles submission of update form for photos |
| /delete/:id |  Delete |             | photoDeleteAction | Handles submission of delete form for photos |



## Mockups


### Desktop Mockup

![Desktop Mockup](https://i.imgur.com/jgK4hQa.png)

### Mobile Mockup

![Mobile Mockup](https://i.imgur.com/PQNSo1c.png) 

### [Deployed Website]()

### [Trello Board](https://trello.com/invite/b/IkEQGiQD/ATTI4be5defd1ea9698676fa47a07ddeb7b59E0B1348/workspace)