# *Jortiz-cyber.github.io*

### *CS499 Computer Science Capstone ePortfolio*

  My name is Jose Ortiz and this is my Computer Science Capstone ePortfolio that will address my three outcomes in Software Design and Engineering, Algorithms and Data Structure, and Databases. This electronic portfolio is meant to provide my information on my completed enhancements of various courses I attended in earning a Bachelor's degree in Information Security.

## *Table of Contents*
1. Professional Self-Assessment
2. Code Review
3. Software Design and Engineering: Pyramids
4. Algorithms and Data Structure: SQL Injection
5. Databases: Tree structure
   
### *Professional Self-Assessment:*

 In completeing this course, I have learned that when enhancing and modifying any artifact I must test and run my code after every modification so that I may correct any errors that appeared with every modification. Saving my source was also an important factor when no errors were present in my code. Adding comments were also important when changes were made so that I may go back and modify the statements to fit my design. Using the same language or standards such as utilizing the same Icon sets when building a website or source codes help maximize my marketing potential in the computer science industry. Researching what many others use as a standard but at the same including individuality and creativity helps market my potential as well. 

 Creating an ePortfolio will help me display my skills and knowledge of what I know and can create or modify. When seeking opportunities in different organizations will require some sort of educational background which is also be something I may display in my ePortfolio. But I do understand that by posting projects or work that I may have created in the past for public consumption can limit the authentication of the source. I also understand that I must limit myself on what can be viewed by the public but at the same time attract an employer for employment. I know that accepting internships and volunteer work will give me hands-on training and will be a good experience to add to a resume.
	
 In this course's outcomes I have achieved on choosing the three artifacts which incorporate my three enhancement plans. The three enhancement plans consist of Software Design and Engineering, Algorithms and Data structures, and Databases. For each enhancement plan I have identified what I would like to enhance and modify which will be descirbed below.

### *Code Review:*

 Below is a video of my code review for this course of my three enhancement file that I have utilized and display my skills.

 https://youtu.be/_POtXL3j95E

### *Enhancement One: Software Design and Engineering*

  The first artifact that I will be enhancing is from course CS-330 of Computational Graphics and Visualization. This design was created in June 19 2023 and consisted of three pyramids on a platform with different textures. I have selected this item because it helps me demonstrate the ability to use innovative techniques, skills, and tools in computing practices that deliver value and accomplished industry specific goals.

  In this artifact I will describe and demonstrate how loops and branches come together to form a visual design that can also be interactive by the user. I will demonstrate how indexes, pointers, and subscripts are tested against arrays. Variables will be defined with meaningful, consistent, and have clear names in each statement. The code in this artifact will be clearly document and easy to read for the next developer that would like to modify this design.

  For this artifact the window width and height were adjusted so that the design can be clearly visualized. The textures of all three pyramids were modified to have a consistent solid color for a better outline of the pyramid. The platform was also modified to display that it may also be changed to match the three pyramids solid textures. I have enhanced this design to meet the course outcomes with building a collaborative environment that enables diverse audiences to support organizational decision making in the field of computer science. I have also designed and developed and delivered professional-quality oral, written, and visual communications that are coherent, technically sound and adapted to specific audiences and contexts.  

 *Original*
  (https://github.com/jortiz-cyber/PyramidsFinal)
  
  *Enhanced*
  (https://github.com/jortiz-cyber/Pyramids-enhanced)

// Window width, height
 
    const int WINDOW_WIDTH = 1240;
    const int WINDOW_HEIGHT = 820;


 ///BUILDING A SHAPE:
	
	//	PYRAMID 01
	GLMesh pyr_mesh_Neonblue;
	pyr_mesh_Neonblue.p = {
		1.0f, 1.0f, 1.0f, 1.0f,				// color r, g, b a
		2.5f, 2.5f, 2.5f,					// scale x, y, z
		0.0f, 1.0f, 0.0f, 0.0f,				// x amount of rotation, rotate x, y, z
		0.0f, 0.0f, 1.0f, 0.0f,				// y amount of rotation, rotate x, y, z
		0.0f, 0.0f, 0.0f, 1.0f,				// z amount of rotation, rotate x, y, z
		0.0f, 0.0f, 0.0f,					// translate x, y, z
		2.0f, 2.0f
	};
	pyr_mesh_Neonblue.height = 0.8f;
	pyr_mesh_Neonblue.texFilename = "textures\\Neonblue.png";
	ShapeBuilder::UBuildPyramid(pyr_mesh_Neonblue);
	scene.push_back(pyr_mesh_Neonblue);
 	
	//	PYRAMID 02
	GLMesh pyr_mesh_Neongreen;
	pyr_mesh_Neongreen.p = {
		1.0f, 1.0f, 1.0f, 1.0f,				// color r, g, b a
		2.5f, 2.5f, 2.5f,				// scale x, y, z
		0.0f, 1.0f, 0.0f, 0.0f,				// x amount of rotation, rotate x, y, z
		0.0f, 0.0f, 1.0f, 0.0f,				// y amount of rotation, rotate x, y, z
		0.0f, 0.0f, 0.0f, 1.0f,				// z amount of rotation, rotate x, y, z
		-1.0f, 0.0f, 4.0f,				// translate x, y, z
		1.0f, 1.0f

	};
	pyr_mesh_Neongreen.height = 0.8f;
	pyr_mesh_Neongreen.texFilename = "textures\\Neongreen.png";
	ShapeBuilder::UBuildPyramid(pyr_mesh_Neongreen);
	scene.push_back(pyr_mesh_Neongreen);

	// PYRAMID 03
	GLMesh pyr_mesh_Neonpink;
	pyr_mesh_Neonpink.p = {
		1.0f, 1.0f, 1.0f, 1.0f,				// color r, g, b a
		2.0f, 2.0f, 2.0f,					// scale x, y, z
		0.0f, 1.0f, 0.0f, 0.0f,				// x amount of rotation, rotate x, y, z
		0.0f, 0.0f, 1.0f, 0.0f,				// y amount of rotation, rotate x, y, z
		0.0f, 0.0f, 0.0f, 1.0f,				// z amount of rotation, rotate x, y, z
		4.0f, 0.0f, -1.5f,					// translate x, y, z
		1.0f, 1.0f
	};
	pyr_mesh_Neonpink.height = 0.8f;
	pyr_mesh_Neonpink.texFilename = "textures\\Neonpink.png";
	ShapeBuilder::UBuildPyramid(pyr_mesh_Neonpink);
	scene.push_back(pyr_mesh_Neonpink);

	// GROUND
	GLMesh mesh;
	mesh.p = {
		1.0f, 1.0f, 1.0f, 1.0f,				// color r, g, b a
		5.0f, 5.0f, 5.0f,					// scale x, y, z
		0.0f, 1.0f, 0.0f, 0.0f,				// x amount of rotation, rotate x, y, z
		0.0f, 0.0f, 1.0f, 0.0f,				// y amount of rotation, rotate x, y, z
		0.0f, 0.0f, 0.0f, 1.0f,				// z amount of rotation, rotate x, y, z
		2.0f, 0.0f, 2.0f,					// translate x, y, z
		1.0f, 1.0f
	};
	mesh.texFilename = "textures\\Neongray.png";
	ShapeBuilder::UBuildPlane(mesh);
	scene.push_back(mesh);
 	}

### *Enhancement Two: Algorithms and Data Structure*

  In my second artifact I have acquired a project from course CS-260 Data Structures and Algorithms that was created on January 20, 2021. In the course of CS-260 I have created a script that retrieved the “eBid_Monthly_Sales.csv” file in the Visual Studio application. The script allows me to load, display, find, and remove any bids from the eBid_Monthly_Sales.csv file. A calculated elapsed time was set in place to determine how much time it took to retrieve an item from this file.
 
 To enhance this algorithm, I have created an algorithm in a different application to open the database file called, "eBid_Monthly_Sales.csv". I have converted the eBid_Monthly_Sales.csv into a .txt file and convert the file to have a different view in the NOTEPAD++ application. I was also able to open a specific item within the file using a more interactive approach.

 I have selected this artifact to help me display my skills in creating a different algorithm by using the same file that was opened in Visual Studio. By using the same structure, I was able to retrieve the same information in a different application. By using a different application I am able to have a different outcome when specifying items from the "eBid_Monthly_Sales.csv" file.

 By meeting the course outcomes and converting the eBid_Monthly_Sales.csv file to a .txt file I was also able to open the file in a different application which would help organizations open my enhanced file various platforms. I was able to minimized the steps on how the file could be retrieved in NOTEPAD++ application.

*Orginal*
(https://github.com/jortiz-cyber/Tree-Structures.git)

*Enhanced*
(https://github.com/jortiz-cyber/Tree-Structure-Enhanced.git)

   	// Load a CSV file containing bids into a container
   	// @param csvPath the path to the CSV file to load
   	// @return a container holding all the bids read
   
    void loadBids(string csvPath, BinarySearchTree* bst) {
    cout << "Loading CSV file " << csvPath << endl;

   	// initialize the CSV Parser using the given path
    csv::Parser file = csv::Parser(csvPath);

   	// read and display header row - optional
    vector<string> header = file.getHeader();
    for (auto const& c : header) {
        cout << c << " | ";
    }
    cout << "" << endl;

    try {
   	// loop to read rows of a CSV file
        for (unsigned int i = 0; i < file.rowCount(); i++) {

   	// Create a data structure and add to the collection of bids
            Bid bid;
            bid.bidId = file[i][1];
            bid.title = file[i][0];
            bid.fund = file[i][8];
            bid.amount = strToDouble(file[i][4], '$');

            cout << "Item: " << bid.title << ", Fund: " << bid.fund << ", Amount: " << bid.amount << endl;

            push this bid to the end
            bst->Insert(bid);
        }
    } catch (csv::Error &e) {
        std::cerr << e.what() << std::endl;
    }
	}
### *Enhancement Three: Databases*

 In my third artifact I have be enhanced a file from course CS-405 Secure Coding. This file was created on January 28,2024 and it’s called, “SQL injection queries”. This script runs various statements and flags errors within a suspected SQL injection. This code runs various queries and selects multiple queries with the correct ID, name, and password from a selected name that has been requested.

 I selected this item because it helped me demonstrate specific skills that will align with the third enhancement requirements which is called, “Databases”. I have add more values to my SQL injection database and test multiple queries at the same time. I was able to run multiple queries with various injections 5 additional times and was able to display many values that need to be queried at once within a SQL injection. 

 I was able to meet the outcomes of my enhancement in this artifact by adding more queries that could be tested. Also added more SQL injections to test multiple queries at the same time with minimal errors. Added three more queries to test my sql injection at the same time and all return with a value of “1 record found” response.

 (https://github.com/jortiz-cyber/SQL-Injection-Enhanced.git)

     // Insert some dummy data
        sql = "INSERT INTO USERS (ID, NAME, PASSWORD)" \
        "VALUES (1, 'Fred', 'Flinstone');" \
        "INSERT INTO USERS (ID, NAME, PASSWORD)" \
        "VALUES (2, 'Barney', 'Rubble');" \
        "INSERT INTO USERS (ID, NAME, PASSWORD)" \
        "VALUES (3, 'Wilma', 'Flinstone');" \
        "INSERT INTO USERS (ID, NAME, PASSWORD)" \
        "VALUES (4, 'Betty', 'Rubble');"\
        "INSERT INTO USERS (ID, NAME, PASSWORD)" \
        "VALUES (5, 'BAMBAM', 'Rubble');"\
        "INSERT INTO USERS (ID, NAME, PASSWORD)" \
        "VALUES (6, 'DINO', 'Flintstone');"\
        "INSERT INTO USERS (ID, NAME, PASSWORD)"\
        "VALUES (7, 'Pebbles', 'Flintstone');"\
        "INSERT INTO USERS (ID, NAME, PASSWORD)" \
        "VALUES (8, 'Mr. Slate', 'Stephenson');";

     // Injected SQLs
        bool run_query_injection(sqlite3* db, const std::string& sql, std::vector< user_record >& records)
        { 
        std::string injectedSQL(sql);
        std::string localCopy(sql);

    // We work on the local copy because of the const
        std::transform(localCopy.begin(), localCopy.end(), localCopy.begin(), ::tolower);
        if (localCopy.find_last_of(str_where) >= 0)
    // This sql has a where clause
        if (localCopy.back() == ';')
        { // smart SQL developer terminated with a semicolon - we can fix that!
            injectedSQL.pop_back();
        }

        switch (rand() % 4)
        {
        case 1:
            injectedSQL.append(" or 2=2;");
            break;
        case 2:
            injectedSQL.append(" or 'hi'='hi';");
            break;
        case 3:
            injectedSQL.append(" or 'hack'='hack';");
            break;
        case 4:
            injectedSQL.append(" or 'inject'='inject';");
            break;
        case 5:
            injectedSQL.append(" or 'damage'='damage';");
            break;
        case 6:
            injectedSQL.append(" or 'break'='break';");
            break;
        case 0:
        default:
            injectedSQL.append(" or 1=1;");
            break;
        }
    }

    return run_query(db, injectedSQL, records);

    // Run Queries
    void run_queries(sqlite3* db)
    {
    char* error_message = NULL;
    std::vector< user_record > records;

    // query all
    std::string sql = "SELECT * from USERS";
    if (!run_query(db, sql, records)) return;
    dump_results(sql, records);

    //  query 1
    sql = "SELECT ID, NAME, PASSWORD FROM USERS WHERE NAME='Fred'";
    if (!run_query(db, sql, records)) return;
    dump_results(sql, records);

    // query 2
    sql = "SELECT ID, NAME, PASSWORD FROM USERS WHERE NAME='Pebbles'";
    if (!run_query(db, sql, records)) return;
    dump_results(sql, records);

    //  query 3
    sql = "SELECT ID, NAME, PASSWORD FROM USERS WHERE NAME='DINO'";
    if (!run_query(db, sql, records)) return;
    dump_results(sql, records);

    //  query 4
    sql = "SELECT ID, NAME, PASSWORD FROM USERS WHERE NAME='Mr. Slate'";
    if (!run_query(db, sql, records)) return;
    dump_results(sql, records);

    //  run query 1 with injection 5 times
    for (auto i = 0; i < 10; ++i)
    {
        if (!run_query_injection(db, sql, records)) continue;
        dump_results(sql, records);
    }

    }
