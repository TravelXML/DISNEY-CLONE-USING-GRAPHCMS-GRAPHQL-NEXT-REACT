# DISNEY CLONE USING GRAPHCMS GRAPHQL NEXT REACT
![DISNEY CLONE USING GRAPHCMS GRAPHQL NEXT REACT](https://user-images.githubusercontent.com/8361967/145450003-b4eadf7e-58c3-49a9-ba72-ba593673ec7b.jpg)

## Build DISNEY Clone using GRAPHCMS, GRAPHQL, NEXT, REACT

### Add assets
First, you need to create your GraphCMS Account then create Assets, Schemas and Contents and their relationships.

![image](https://user-images.githubusercontent.com/8361967/145436231-6fa3ce18-430a-4ff0-9139-9d68e009ccbe.png)

### Playground

Once you are done with Schema and relation building, build  GQL queries for data fetching and mutation.

### Example: 

### Below one to fetch all videos with specific details.

            query {
                  videos {
                    createdAt,
                    id,
                    title,
                    description,
                    seen,
                    slug,
                    tags,
                    thumbnail {
                      url
                    },
                    mp4 {
                      url
                    }
                  }
                }
                
### Fetch Specific Video by unique id

            query{
              videos(where: { id:"ckwyfg18o096k0c05j5bw1bl5"}){
                createdAt,
                id,
                title,
                description,
                slug,
                tags,
                thubnail{
                  url
                },
                mp4{
                  url
                }
              }
            }
                
### Fetch Account Details

            query {
                account(where: { id: "ckwyfc4t4096b0c184nqkh2zq"}) { 
                  username
                  avatar {
                    url
                  }
                }
              }

For more reference you can have a look into the image below.

![image](https://user-images.githubusercontent.com/8361967/145438884-1f4948a7-a786-4881-99bb-88b6a6e6adec.png)



### Add a .env file

After the assets are loaded, add a .env file in root folder with the following:

![image](https://user-images.githubusercontent.com/8361967/145437044-5a64ddd8-1a5f-475f-962a-b40e0d4626b8.png)

    GRAPH_CMS_TOKEN={your_token}

    ENDPOINT={your_endpoint}

![image](https://user-images.githubusercontent.com/8361967/145436729-8ea993df-e10a-4bce-92af-e8043269a405.png)
 


### Run the command below to install the packages.

    npm i


### Run the development server:

    npm run dev
 
 
  ![image](https://user-images.githubusercontent.com/8361967/145437311-7926b265-6fb9-406d-9b40-cad5e5508c4a.png)  
 


 
Open http://localhost:3000 with your browser to see the result.

![image](https://user-images.githubusercontent.com/8361967/145438318-62b43392-7844-492e-a9e2-4fd683fc4329.png)


You can start editing the page by modifying pages/index.js. The page auto-updates as you edit the file.


**Enjoy Coding!**



