# React Challenge


## 1 - Mern-seed  login research:
Clone the mern-seed project.  
Create a branch from master following our github conventions in case you want to implement the feature or just add comments/suggestions of the code that you look.
If we decided to implement a login form into the project, what will be the best approach to take? You can create a comparison table of the possible options and make a conclussion with what will be for you the best decision to take (assume that the client has an amazing API)

Bonus track: implement the login based on your decision and made a PR with your changes

![](https://content.screencast.com/users/mravinales/folders/Jing/media/54554999-375c-4b76-9c4a-2d67ce26424c/00000650.png)

## 2 - Mern-seed login with JWT:
Clone the mern-seed project.  
Create a branch from master following our github conventions.
Implement a basic login using JWT.
Create a PR with your code so others devs can made a code review on it.

![](https://content.screencast.com/users/mravinales/folders/Jing/media/54554999-375c-4b76-9c4a-2d67ce26424c/00000650.png)

## 3 - Mern-seed grid research:
Clone the mern-seed project.  
Create a branch from master following our github conventions in case you want to implement the feature or just add comments/suggestions of the code that you look.
If we decided to implement a grid into the project, what will be the best approach to take? You can create a comparison table of the possible components around there and make a conclussion with what will be for you the best decision to take.

Bonus track: implement the grid component based on your decision and made a PR with your changes
![](http://www.independent-software.com/wp-content/uploads/2014/03/ajax-table-example.png)

## 4 - Mern-seed grids:
Clone the mern-seed project.  
Create a branch from master following our github conventions.
Create a new page in the project
Implement a grid component. 
Create a grid with the following format:

![](http://www.independent-software.com/wp-content/uploads/2014/03/ajax-table-example.png)

The object what you will get from the API will be something like this:
 [ 
   {id: 1, name: 'Brampton Sauvignon Blanc', hasStock: false},
   {id: 10, name: 'Le Riche Cabernet Sauvignon', hasStock: true},
   {id: 11, name: 'Vergelegen', hasStock: false},
   {id: 12, name: 'Veenwouden Merlot', hasStock: true},
   {id: 13, name: 'De Trafford Pinot Noir', hasStock: true},
   {id: 14, name: 'De Wetshof Pinot Noir', hasStock: true},
   {id: 15, name: 'De Wetshof Limelight Chardonnay', hasStock: true},
   {id: 15, name: 'De Wetshof Pinor Noit Brut', hasStock: true}
]
You only need to display in the grid the ones that has stock

## 5 - Google map challenge:
This test should take about an hour to do. 

Fork the following JSFiddle that has the base data:

https://jsfiddle.net/mravinale/Lyy64nwc/


Create an react app (In js fiddle) that does the following:

Uses a data service to get the data from the object in the fiddle above

Use (http://doc.jsfiddle.net/use/echo.html) to make the get statement on the http service.


#### Handles the data in a way that produces something that fits the followings rules:

The array of listings need to show in the order given by the data service.

- For the Price

  * It should have "$" and commas as separators.

  * If the Transaction is Rent, then it should also say "per month" after it

- Open Houses are to look like:

  * Open House: Feb. 3rd - 2:00 AM to 3:30 PM

  * Only show the next open house that is to occur.

- The overall format of the listing:

  * First line: Left Align Street Number + Street Name, right align price.

  * Second Line: Left Align Transaction

  * Third+ Lines: Open Houses centered in the format given above

Below the results, in a map that is 400x400, geocode the 2 addresses with google maps.

The JsFiddle has gmaps loaded as an external resource if you fork it.

Clicking the marker for a listing, should highlight that listing in the results. 


## Bonus 
Given the following code, can you identify the two main problems? 

class MyComponent extends React.Component {
    constructor(props) {
        // set the default internal state
        this.state = {
            clicks: 0
        };
    }

    componentDidMount() {
        this.refs.mainContainer.addEventListener(
            ‘click’, 
            this.clickHandler
        );
    }

    componentWillUnmount() {
        this.refs.mainContainer.removeEventListener(
            ‘click’, 
            this.clickHandler
        );
    }

    clickHandler() {
        this.setState({
            clicks: this.clicks + 1
        });
    }

    render() {
        let children = this.props.children;

        return (
            <div className=”main-container” ref=”mainContainer”>
                <h2>My Component ({this.state.clicks} clicks})</h2>
                <h3>{this.props.headerText}</h3>
                {children}
            </div>
        );
    }
}




Everything will be evaluated, technical and non-technical skills. Show us what you've got!

Tip: if you don't know something make your best guess or assumption, we want to know how you think.

Remember: Create a new repository for your project. When you are ready, send it to us so we can check it out!

The Development Team wishes you luck, and we hope to have you working with us soon!

May the code be with you.
