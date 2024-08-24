---
layout: default
---

[Link to another page](./another-page.html).

# Professional Self-Assessment
* * *
  My name is Ryan Miller. I started my Computer Science journey at Navarro College in Corsicana Texas in 2020. I received my A.S. in Computer Science from Navarro College in the fall of 2021. I then began working on my B.S. in Computer Science at Southern New Hampshire University in the fall 2022. I have a great deal of appreciation for both of the institutions I attended. Learning through two different approaches to computer science education has made me a more versatile engineer as I have my education has been equal parts practical and theory. Along the way, I have gained new skills and improved upon old ones. I have become increasingly detail oriented and mindful of best practices in my work. I have become proficient in multiple languages, including Java, C++, and Python. I have gained skills in database management and project planning. I am appropriately cautious in my approach to development, testing as I go, and I have become quite skilled at tracking down issues and bugs in my own code and in the work of others. I try to apply professional security standards in my work where possible, this makes up a big part of best practice to me and I try to implement security solutions in my work wherever I see a need. I do my best to keep all of my work well commented, organized, and easy to follow. I enjoy taking part in peer review processes, having my code reviewed and reviewing the code of others. 

  During my time at SNHU, I took a course that focused on the importance of version control in project development. It involved a class wide group project where every student was responsible for adding a given feature one piece at a time on their own branch, and continually remerging back into the main branch with the rest of the class. This required class wide code reviews. This experience was very valuable because it was one of the first times I had the opportunity to work on a project with such a large group of people while also having the ability to make suggestions, approve or deny pull requests. I was able to really dig into other developers’ code, analyze conflicts, and do my part to ensure everything continued to go smoothly. 

  As an engineer, I place great value in clarity. It is very important to me that I fully understand the needs and requirements of a project. I try not to make assumptions and I will always reach out first if a conflict or issue arises in order to ensure that the client/stakeholders are getting the solution they need. I received frequent praise for this value when I was studying at Navarro College. There were multiple instances in which project requirements were unclear and only a few of us chose to reach out to a professor or other “stakeholder” in the project for clarity. Usually this resulted in a program that actually solved the problem, while much of the rest of the class had made assumptions that had either limited the functionality of their solution or fell short of the project requirements. 

  To help showcase my skills and everything I have learned over the last four years, I have selected three artifacts from my time at SNHU. These are all final projects from courses I completed, and the enhancements I have made to them will highlight my competence across the following outcomes:

*   Employ strategies for building collaborative environments that enable diverse audiences to support organizational decision making in the field of computer science
  
*   Design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts
  
*   Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution, while managing the trade-offs involved in design choices
  
*   Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals
  
*   Develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources

I have taken many classes throughout my time in this program, but the courses I selected artifacts from where all courses in which I either learned something very new and challenging, or cases in which I felt I could have taken my work much further but didn’t for lack of time or scope. These artifacts include a C++ program that was translated to Java and then reformatted as a GUI, an OpenGL program in which I wrote and implemented an algorithm to dynamically generate and texture cylinders, and an Android mobile application for inventory management in which I refactored the existing database solution to tie entries to user accounts and provide support of sorting and searching functions on the database screen. These artifacts provide weight to this portfolio by clearly presenting my aforementioned skills in one place, without the need to download, examine, and run these applications yourself (though you can).


# Code Review
* * *

# Original Artifacts
* * *
### Software Engineering and Design
The C++ program I selected for enhancement is a program that I reverse engineered from legacy code as part of the final project for CS 410 Software Reverse Engineering. It is a simple program that runs in a terminal window. It is designed to allow “SNHU Investments”, a fictional investment company that offers brokerage and retirement services, to view and edit the service options they offer to specific clients.

The following image illustrates a sample of the terminal output and user input for this artifact in its original state:

![SED_Old](https://github.com/RyanJMiller/RyanJMiller.github.io/blob/main/assets/SED_Old.png)

This repository for this artifact can be found HERE.

### Algorithms and Data Structures
The OpenGL project I selected for enhancement is my final project from CS 330 Computational Graphics and Visualization. The project was created using Visual Studio The project is composed of a single source cpp file and 5 images used as textures for 3D objects. When run, it draws a navigable 3D scene with a several 3D shapes representing an orange, a measuring cup, and a digital camera all sitting on a paper towel. One important note here is that while the points for the sphere are generated using for loops, the cylinders are all literally defined and very low-poly cylinders as a result.

The following images display the 3D scene:

![ADS_Old](https://github.com/RyanJMiller/RyanJMiller.github.io/blob/main/assets/ADS_Old.png)

Part of the original function used to literally define the points of the cylinder (around 300+ lines in full):

```c++
// UCreateCylinder function
void UCreateCylinder(GLMesh& mesh)
{
    // point positions and colors
    GLfloat verts[] = {
        // vertex positions   // normals         // texture coordinates
         1.0f,  0.0f,  0.0f,  1.0f, 0.0f, 0.0f,  0.5f, 0.5f, // front face Vertex 0
         1.0f, -0.2f,  1.0f,  1.0f, 0.0f, 0.0f,  0.4f, 1.0f, // front face Vertex 1
         1.0f, -0.5f,  0.9f,  1.0f, 0.0f, 0.0f,  0.25f, 0.95f, // front face Vertex 2
         1.0f,  0.0f,  0.0f,  1.0f, 0.0f, 0.0f,  0.5f, 0.5f, // front face Vertex 0
         1.0f, -0.5f,  0.9f,  1.0f, 0.0f, 0.0f,  0.25f, 0.95f, // front face Vertex 2
         1.0f, -0.75f, 0.75f, 1.0f, 0.0f, 0.0f,  0.125f, 0.875f, // front face Vertex 3
         1.0f,  0.0f,  0.0f,  1.0f, 0.0f, 0.0f,  0.5f, 0.5f, // front face Vertex 0
         1.0f, -0.75f, 0.75f, 1.0f, 0.0f, 0.0f,  0.125f, 0.875f, // front face Vertex 3
         1.0f, -0.9f,  0.5f,  1.0f, 0.0f, 0.0f,  0.05f, 0.75f, // front face Vertex 4
         1.0f,  0.0f,  0.0f,  1.0f, 0.0f, 0.0f,  0.5f, 0.5f, // front face Vertex 0
         1.0f, -0.9f,  0.5f,  1.0f, 0.0f, 0.0f,  0.05f, 0.75f, // front face Vertex 4
         1.0f, -1.0f,  0.2f,  1.0f, 0.0f, 0.0f,  0.0f, 0.6f, // front face Vertex 5
         1.0f,  0.0f,  0.0f,  1.0f, 0.0f, 0.0f,  0.5f, 0.5f, // front face Vertex 0
         1.0f, -1.0f,  0.2f,  1.0f, 0.0f, 0.0f,  0.0f, 0.6f, // front face Vertex 5
         1.0f, -1.0f, -0.2f,  1.0f, 0.0f, 0.0f,  0.0f, 0.4f, // front face Vertex 6
         1.0f,  0.0f,  0.0f,  1.0f, 0.0f, 0.0f,  0.5f, 0.5f, // front face Vertex 0
         1.0f, -1.0f, -0.2f,  1.0f, 0.0f, 0.0f,  0.0f, 0.4f, // front face Vertex 6
         1.0f, -0.9f, -0.5f,  1.0f, 0.0f, 0.0f,  0.05f, 0.25f, // front face Vertex 7
         1.0f,  0.0f,  0.0f,  1.0f, 0.0f, 0.0f,  0.5f, 0.5f, // front face Vertex 0
         1.0f, -0.9f, -0.5f,  1.0f, 0.0f, 0.0f,  0.05f, 0.25f, // front face Vertex 7
         1.0f, -0.75f, -0.75f,  1.0f, 0.0f, 0.0f,  0.125f, 0.125f, // front face Vertex 8
         1.0f,  0.0f,  0.0f,  1.0f, 0.0f...
```

This repository for this artifact can be found HERE.

### Databases
The Android mobile application I selected for enhancement is sourced from my final project from CS 360 Mobile Architecture and Programming. When deployed on an Android device, this application will allow you to register an account with a password and username, login, and create, edit, and delete inventory entries. Unfortunately, the original artifact allows any logged in user to view and modify the same set of entries even if they were created on another user's account.

The following image displays the original inventory screen:

![Databases_Old](https://github.com/RyanJMiller/RyanJMiller.github.io/blob/main/assets/Databases_Old.jpg)

Inventory database queries:

```java
@Dao
public interface InventoryDao {

    // Query to retrieve all items from the inventory_items table
    @Query("SELECT * FROM inventory_items")
    LiveData<List<Inventory>> getAllItems();

    // Insert a new item into the inventory_items table
    @Insert
    void insertItem(Inventory inventory);

    // Update an existing item in the inventory_items table
    @Update
    void updateItem(Inventory inventory);

    // Delete an item from the inventory_items table
    @Delete
    void deleteItem(Inventory inventory);
}
```

This repository for this artifact can be found HERE.

# Enhancements
* * *

### Software Engineering and Design
The simplicity of the first artifact meant, to me, that it would be the easiest to do more with. I could expand upon it and take the oppurtunity to learn some new things without being concerned about the project being too much work for the time table. Ultimately I chose to first translate the C++ program into Java, retaining the original functionality of the program, and then replace the terminal window interface loop with a GUI to simplify the experience for the user using the Javax Swing library. Additionally, there were issues with the existing login system. The original artifact had the password stored in plain text as a string within the program. I enchanced the login feature by first salting and then hashing the original password and then storing the salt and hash as attributes under an Account class. I added thorough input validation on the username and password fields, and created several methods to handle login authentication. Finally, I ensured that the whole application was properly subdivided and organized into different java files and packages. All of the classes related to user authentication and input validation are contained in a util (utilities) package, the Account class is stored in a models package, and the driver file as well as all of the classes associated with the different screens of the GUI are stored together. In it's completed state, the application now has more secure login authentication, includes an easy to use main screen that lists all of the clients and allows the user to edit the selected service option for any client. 

These enhancements demonstrate my proficiency in translating a program from one programming language to another and in user friendly GUI development. These enhancements not only improved the usability of the system but also ensured that all functionalities from the original program were retained and even enhanced. By translating the program from C++ to Java, I demonstrated my ability to design and evaluate computing solutions to ensure the functionality and performance of the system. I also ensured that the new artifact is well commented and easy to follow. Implementing user authentication and following best practices highlighted the importance of a security mindset during the development process.

The following is an image of the main screen where users can make edits to client service selections:

![SED_New](https://github.com/RyanJMiller/RyanJMiller.github.io/blob/main/assets/SED_New.png)

This repository for this artifact can be found HERE.

### Algorithms and Data Structures
Prior to enhancement this artifact contained functions that literally defined the position of the points and triangles needed to draw cylinders. This involved specifying the coordinate locations for each and every point in the 3D shape line by line. This is both an inefficient time-consuming process. In an effort to improve the cylinder generation function and make it possible to upscale the polygonal resolution of the cylinder just by changing a few values, I chose to define an algorithm that would dynamically generate and texture the points and triangles of the cylinder based on a few easily changed values that determine the shape's polygonal resolution. This process involved properly managing and storing all of the relevant generated point data for the cylinder. Additionally, I decided to break up and reorganize the original single cpp file into a series of header files and implementations that allowed me to move the functions for mesh generation, shader creation/destruction, and texture creation/destruction into their own separate files. The result was better looking and hi poly shapes that helped better communicate the representation of each object in the scene, and a more well organized and easier to follow project architecture.

These enhancements demonstrate my ability to apply algorithmic solutions and manage data structures in a practical context, improving the overall quality and performance of the program. I had to develop an algorithm for dynamic shape generation, efficiently manage and store the generated vertices, and demonstrate an understanding of more advanced OpenGL concepts.

The following is an image of the 3D scene after making the enhancements:

![ADS_New](https://github.com/RyanJMiller/RyanJMiller.github.io/blob/main/assets/ADS_New.png)

First part (for the sake of brevity) of the new function used to generate and texture the points of the cylinder:

```c++
void UCreateCylinder(GLMesh& mesh) {
    const int segments = 36;
    const float radius = 1.0f;
    const float height = 2.0f;
    std::vector<GLfloat> vertices;
    std::vector<GLuint> indices;

    float angleStep = 2.0f * glm::pi<float>() / segments;

    // Generate vertices and normals
    for (int i = 0; i <= segments; ++i) {
        float angle = i * angleStep;
        float x = radius * cos(angle);
        float z = radius * sin(angle);
        float u = (float)i / segments;

        // Top vertex
        vertices.push_back(x);                // x
        vertices.push_back(height / 2.0f);    // y
        vertices.push_back(z);                // z
        vertices.push_back(x);                // normal x (for smooth shading, use x and z)
        vertices.push_back(0.0f);             // normal y
        vertices.push_back(z);                // normal z
        vertices.push_back(u);                // texture u
        vertices.push_back(1.0f);             // texture v

        // Bottom vertex
        vertices.push_back(x);                // x
        vertices.push_back(-height / 2.0f);   // y
        vertices.push_back(z);                // z
        vertices.push_back(x);                // normal x (for smooth shading, use x and z)
        vertices.push_back(0.0f);             // normal y
        vertices.push_back(z);                // normal z
        vertices.push_back(u);                // texture u
        vertices.push_back(0.0f);             // texture v
    }
```

This repository for this artifact can be found HERE.

### Databases
This application was originally created to allow users to register for and sign into accounts and keep track of various inventory entries. The original program solved this problem in a simple sense, but there were some issues, namely when a user registered and logged into their account, they would have access to inventory items added and edited by other accounts. Additionally, the inventory management screen did not have any of the basic search and sorting functions that consumers have come to expect from tools that allow them to keep track of and analyze lists of items. I enhanced this application by first refactoring the inventory database and queries, that I had previously built using Room, to add a user ID field to inventory item entries and allow the user ID to be used as a means for filtering the inventory item entries so that whenever a user logged in to their account, they would only see the entries that have their user ID tied to them. I then refactored the login process to pull the user ID upon login, and pass it to the class for the inventory screen so that the currently logged in user can be persistently tracked. I then added queries to the inventory database to support search and sorting functionality, and then added the needed search bar and drop down menu to the inventory screen UI.

These enhancements highlight my proficiency in designing database solutions and managing and improving upon an existing DBMS. I also felt that the enhancements would demonstrate a security mindset in my work and specifically in properly securing the data entered and edited by individual users. These enhancements not only improved the usability of the inventory management application but also ensured that user entries would be better protected from tampering by other accounts. From the moment a user logs in, their unique ID is tracked and used across the program to ensure that they only have access to their information. There are some minor tweaks I still want to make in polishing, including one issue I discovered late in testing where setting a sorting option and then using the search function can cause the items to revert to listing in ascending order by their item ID numbers, and this breaks the selected sort option until another sort option is selected. Overall though I believe I was able to clearly demonstrate my proficiency in database management, Android development, and UI design.

The following is an image of the enhanced inventory screen:

![Databases_New](https://github.com/RyanJMiller/RyanJMiller.github.io/blob/main/assets/Databases_New.jpg)

Enhanced Inventory queries:

```java
@Dao
public interface InventoryDao {

    // Query to retrieve all items for the current user
    @Query("SELECT * FROM inventory_items WHERE user_id = :userId")
    LiveData<List<Inventory>> getItemsForUser(int userId);


    // Search items by name
    @Query("SELECT * FROM inventory_items WHERE user_id = :userId AND item_name LIKE '%' || :searchQuery || '%'")
    LiveData<List<Inventory>> searchItemsByName(int userId, String searchQuery);

    // Sort items by name in ascending order
    @Query("SELECT * FROM inventory_items WHERE user_id = :userId ORDER BY item_name ASC")
    LiveData<List<Inventory>> getItemsForUserSortedByNameAsc(int userId);

    // Sort items by name in descending order
    @Query("SELECT * FROM inventory_items WHERE user_id = :userId ORDER BY item_name DESC")
    LiveData<List<Inventory>> getItemsForUserSortedByNameDesc(int userId);

    // Sort items by quantity in ascending order
    @Query("SELECT * FROM inventory_items WHERE user_id = :userId ORDER BY quantity ASC")
    LiveData<List<Inventory>> getItemsForUserSortedByQuantityAsc(int userId);

    // Sort items by quantity in descending order
    @Query("SELECT * FROM inventory_items WHERE user_id = :userId ORDER BY quantity DESC")
    LiveData<List<Inventory>> getItemsForUserSortedByQuantityDesc(int userId);


    // Insert a new item into the inventory_items table
    @Insert
    void insertItem(Inventory inventory);

    // Update an existing item in the inventory_items table
    @Update
    void updateItem(Inventory inventory);

    // Delete an item from the inventory_items table
    @Delete
    void deleteItem(Inventory inventory);
}
```

This repository for this artifact can be found HERE.
 
# Artifact Narratives
* * *


## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```java
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
