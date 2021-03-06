# TUD Cyber Analytics Lab

This is the repository for the CA lab's website. It is deployed using `github.pages` and borrows open source themes. 

### Usage

#### Adding a new member
1. Add the member's picture in the `/assets/people/` folder.
2. Make a file with the member's information (name, position, etc.) and place it in the `_people` folder (Changes in `_config.yml` are no longer supported).
3. Fill the filename in `pic` field,
4. and assign them a role from the given `roles` collection in `_config.yml`. You can even add a new role.
5. Optionally, also add the links to their personal webpage.
6. Commit the changes.

#### Adjusting picture size
1. Open powerpoint and insert your picture from the `Insert` menu
2. Select `Crop` -> `Aspect rartio` -> `1:1` and adjust the cropped area
3. Then, select `Crop` -> `Crop to shape` -> `Oval`
4. Finally, right-click, choose `Save as picture`, and store it in the `assets/people/` folder.

#### Structure

##### Folders
- `_data`: Contains the configuration file for fonts and the color scheme for the website text
- `_includes`: Whenever some `.html` content needs to be rendered in `.md` file, the `.html` goes here. It also contains `/css/agency.css` file with the primary style guide for the whole website. 
- `_layouts`: Contains the various layouts (templates) for the webpages, e.g. how the project entries, and the team page will render. These files contain a mix of `Jekyll` and `HTML` code.
- `projects`: Contains the file that renders the project page containing a collection of project entries. 
- `_posts`: The individual entries for each project are contained here. The file names typically follow the follwing format `%YYYY-%MM-%DD-projectname.md`. We don't render the dates anymore.
- `_people`: The team members' information is placed in this folder. One file for each person.
- `assets`: Contains images and scripts used by the webpages.
- `css`: Contains font-awesome style guides
- `js`: Contains the jQuery and Bootstrap scripts for stylizing the webpages.

##### Files
- `_config.yml`: The main configuration file. It contains the navigation layout, the group name, and specifies the collection used by project, papers and team entries. It also contains the theme related information, i.e. the Jekyll plugins and settings used.
- `index.md`: This is the Home page when the website is loaded
- `people.md`: This is the page called when the _People_ link is clicked. This page calls the layout and other files to render the Team page.
- `contact.md`: This page is called when _Contact_ link is clicked. This page calls the layout and other files needed to render the Contact us page properly.
- `categories.md`: If a project categy is clicked, all related projects are shown. This page calls the layout and other script to make that happen.


