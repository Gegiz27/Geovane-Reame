# Geovane-Reame

unsigned int theVAO; // Nome do Vértice Array Objeto (VAO)

glGenVertexArrays (1,&theVAO);

unsigned int theVBO; // Nome do Vértice Buffer Objeto (VBO)

glGenBuffers (1, &theVBO);

glBindBuffer (GLARRAYBUFFER,theVBO); // Selecione o VBO ativo

glBufferData (GLARRAYBUFFER, sizeof(verts), verts, GLSTATICDRAW);

unsigned int vPos loc = 0; // Localização do shader

glBindVertexArray(theVAO); // Selecione o VAO ativo

glVertexAttribPointer (vPos loc, 2, GL_FLOAT, GL_FALSE, 0,(void*)0 );

glEnableVertexAttribArray(vPos loc);
