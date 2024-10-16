# *Jortiz-cyber.github.io*

### *CS499 Computer Science Capstone ePortfolio*

  My name is Jose Ortiz and this is my Computer Science Capstone ePortfolio that will address my three outcomes in Software Design and Engineering, Algorithms and Data Structure, and Databases. This electronic portfolio is meant to provide my information on my completed enhancements of various courses I attended in earning a Bachelor's degree in Information Security.

## *Table of Content*
1. Professional Self-Assessment
2. Code Review
3. Software Design and Engineering: Pyramids
4. Algorithms and Data Structure: SQL Injection
5. Databases: Tree structure
   
### *Professional Self-Assessment:*
### *Code Review*
### *Enhancement One: Software Design and Engineering*

  The first artifact that I will be enhancing is from course CS-330 of Computational Graphics and Visualization. This design was created in June 19 2023 and consisted of three pyramids on a platform with different textures. I have selected this item because it helps me demonstrate the ability to use innovative techniques, skills, and tools in computing practices that deliver value and accomplished industry specific goals.

  In this artifact I will describe and demonstrate how loops and branches come together to form a visual design that can also be interactive by the user. I will demonstrate how indexes, pointers, and subscripts are tested against arrays. Variables will be defined with meaningful, consistent, and have clear names in each statement. The code in this artifact will be clearly document and easy to read for the next developer that would like to modify this design.

  For this artifact the window width and height were adjusted so that the design can be clearly visualized. The textures of all three pyramids were modified to have a consistent solid color for a better outline of the pyramid. The platform was also modified to display that it may also be changed to match the three pyramids solid textures. I have enhanced this design to meet the course outcomes with building a collaborative environment that enables diverse audiences to support organizational decision making in the field of computer science. I have also designed and developed and delivered professional-quality oral, written, and visual communications that are coherent, technically sound and adapted to specific audiences and contexts.

   When enhancing and modifying this artifact I have learned that I must test and run my code after every modification so that I may correct any errors that appeared with every modification. Saving the source was also an important factor when no errors were present. Adding comments were also important when changes were made so that I may go back and modify the statements to fit my design. The challenges I face were modifying the interactive statements that allowed me to switch from mouse operation to keyboard stroke operations.

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

### *Enhancement Two: Algorithms and Data Structure*
### *Enhancement Three: Databases*
