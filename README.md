# Mesh_Demo

Welkom bij de Readme voor de Experience voor SURE for ArcGIS. Hierin wat uitleg over waar wat gevonden kan worden. 

----------------------------------------------------------------------------------------------------

Voor vragen kan je mij bereiken op:
nielscramer@hotmail.com

----------------------------------------------------------------------------------------------------

In **Videos** staan 3 videos: 

- BIM2
- Dakwerkzaamheden
- Evenementen

Deze 3 videos zijn use cases voor de 3D Integrated Meshes. 

----------------------------------------------------------------------------------------------------

In **Assets** staan GlTF Modellen. Deze worden gebruikt in Evenementen.html

----------------------------------------------------------------------------------------------------

In **HTML** staan een aantal HTML bestanden. Deze worden gebruikt voor de SURE experience, maar zijn
ook gebruikt voor mijn stageonderzoek naar gebruikerswensen voor 3D Integrated meshes. 

---------------------------------------------------------------------------------------------------

- **BIM_Mesh.html:**			Mesh edits en BIM model plaatsen. Voor SURE en onderzoek.

- **Evenementen.html:**		Event planner met de GlTF modellen

- **Line_of_sight.html:**		Alleen een Line of Sight app. REDACTED

- **Meten_punt_werkzaamheden.html**:		Survey123 + Mesh. Gebruikt voor SURE en onderzoek.


- **Table_Overlap.html**:		Tabel voor SURE

- **Table_Processing.html:**		Tabel voor SURE

- **Viewer.html:**			Kale viewer voor SURE en Onderzoek.

- **mgi_survey.htm**l			Survey123 + Mesh + Meten. Gebruikt voor onderzoek.

----------------------------------------------------------------------------------------------------

**Hoe aanpassen?**

In het script staat een stuk die de mesh ophaalt. Deze ziet er zo uit. 

        // Create SceneLayer and add to the map
        const meshLayer = new IntegratedMeshLayer({
          portalItem: {
            id: "a0763af4aee24afd8ac299e31dfbd7fb"
          },
          popupEnabled: false
        });
        

Vervang **id** met het id van de mesh die je wilt gebruiken. 
  
 
        const view = new SceneView({
                container: "viewDiv",
                map: map,
                camera: {
                position: [5.139278, 52.339105, 100],
                tilt: 45,
                heading: 0
                }
                });

Vervang de **camera position** met de latitude en longitude.
