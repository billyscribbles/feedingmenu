### Run

To run backend navigate to FeedingMenu\API than run the following command:

- dotnet watch run

### Git

Checks the status

- git status

Creates a empty repository

- git init

Will track all files inside the repository and stage the changes

- git add .

Comming staged changes into source control

- git commit -m "Initial Commit"

To push the source control into github for file sharing

- git push -u origin main

### Data Migration

If Entity Framework tools version is older than that of the run time please update to correct version via:
dotnet tool update --global dotnet-ef --version 5.0.0

We update DataContext.cs to create tables and you can also add data here
We update Seed.cs to insert specific value for specific tables
Everytime you make changes to code you need to generate migration code to create a new scaffold version using the command below:

This command creates files inside Persistence > Migrations which is used to scaffold our database , run at root level.
dotnet ef migrations add "Name of Migration" -p Persistence/ -s API/

Running the application will automatically update the database with each migration iteration to the latest migration.
Navigate to FeedingMenu\API and run: dotnet watch run

### Useful References

To comment please use the following:
Shift + Alt + A for comment block

- \* Important information is highlighted
- ! Alert
- ? Questions
- TODO: to do task
