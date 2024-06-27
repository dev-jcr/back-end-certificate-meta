#### Main Backend areas
    Webserver
    Database
    Architecture

### Generally needed skills/languages
    Back-end language
    Database
    APIs
    Web servers

### Website process
    Planning
    Architecture
    Design
    Development
    Deployment
    Maintenance

### Browser inner workings
    Continuous Request-Response Cicle

### Hosting
    Shared
        Small
        Practice
        Free
    VPS
        Allocated virtual capacity
    Dedicated physical server
        Allocated physical capacity
    Cloud
        Combines Virtual and physical 
            Better reliability and performance
        
## Internet Protocols
    IP
        Addresses
            V4
                4 octets
            V6
                8 groups of 4 hexadecimal digits
        Packet
            Problems
                Arrive out of order
                Become damaged or corrupted
                Dropped or lost during transit
            Content
                Destination IP
                Source IP
                Payload
                    Data
                    Transmission Protocols
                        TCP - Transmission Control Protocol
                            Solves problems at the cost of speed.
                        UDP - User Datagram Protocol
                            Faster but doesn't solve data lost.
### HTTP
    It is
        Core protocol of the WWW
        HyperText Transfer Protocol
    Composed of
        Method 
            Type of action the client must perform. Most used:
                GET
                    Retrieve resource
                POST
                    Send data
                PUT
                    Substitute resource
                DELETE
                    Deletes resource
        Path 
            Full path of a particular file on the web server
                /example.com/img.jpg
        Version
            1.1 and 2 the most used
                HTTP/x.x    
        Headers
            Contains addittional information about the request.
                Host
                    specifies the host of the server and indicates where the resource is being requested from.
                User-Agent
                    informs the web server of the application making the request. Operating system (Windows, Mac, Linux), version and vendor of the application.
                Accept
                    tells the web server what type of content the client will accept as a response
                Accept-Language
                    indicates the language and, optionally, the locale that the client prefers
                Content-type
                    indicates the type of content that is transmitted in the body of the request.
        Message Body
            Used when POST and PUT used containing data inside brackets
    HTTP Answer
        First line
            Status codes
                On the first line proceeded by a text representation
                    200 OK
                    404 Not Found
                Five groups
                    Informational 100-199
                        Provisional responses sent by the server
                        100 Continue        
                    Successful 200 -299
                        Request successfully processed
                        200 OK
                    Redirection 300 - 399
                        The resource has been moved
                        301 Moved Permanently
                        302 Found
                    Client error 400 - 499
                        The request contains bad sintax or content 
                        400 Bad Date 
                        401 User must log
                        403 Not enought permission
                        404 Resource Not Found
                    Server error 500 - 599
                        Failure on the website while trying to process
                            500 Internal server error
        Common second liners
            Date
                Date and time of the answer
            Server
                Software of the server used to answer
            Content-Lenght
                Size of answer
            Content-Type
                Type of resource returned
        Body of the answer
            Last part of the answer with content answered
                Images
                Video
                Documents HTML
                Others
    HTTPS
        Encrypted version of HTTP
### DHCP
    Dynamic Host Configuratio Protocol
        Using UDP the clients contacts the server
            The server has registry of connected devices
            Assigns a new one and answers with It

### DNS
    Dynamic Name system
        It provides the info of the IP related to the domain

### IMAP
    Used to retrieve email

### SMTP
    Used to send email.

### POP
    Old protocol that deletes emails when downloaded from the server

### FTP
    File Transfer Protocol

### SSH
    Secure Shell

### SFTP
    Encrypted data transmission trough SSH

### Developer Tools
    Console Tab
        Outputs javascript logs and errors
    Sources
        All content result
    Network
        Inspect the timeline and details of HTTP requests
    performance
        shows what the browser is doing over time
            can help to pinpoint functions slowing down the webapp
    memory
        the codes consuming the more resources
    elements
        Inspect elements
            right panel shows the details


### Frameworks
    Provide structure
    Opinionated
    Call libraries

### Libraries
    Provide reusable pieces of code
    Non-opinionated

### APIs
    Examples
        Browser API
            DOM API
            Geolocation API
            Fetch API - Data
            Canvas API - Graphics
            History API
            Web storage API
            RESTful API
        Web API
        Sensor base API
            Smartlights
    Have
        Endpoints
            Like: https://example.com/?=info
        Server side actions
            Processing and answer
                often in JSON and XML
### REST
    A set of principles used to build highly efficient APIs
    RESTful API
        GET
        POST
        PUT
        DELETE

### HTML
    Origin
        Born in 1991 by Tim Berners Lee
        W3C regulates standard
    Basic structure
        doctype > (html (head(title) (body))
    
    Structures
        Table
            <table>
                <tr>
                    <th> Header 1 </th>
                    <th> Header 2 </th>
                </tr>
                <tr>
                    <td> Column 1 Item 1 </td>
                    <td> Column 2 Item 2  </td>
                </tr>
        Form
            Password
                <form action="/registration" method="POST">
                    <label> for = "username">Username:</label><br>
                    <input type = "text" name="username">

                    <label> for = "password">Password:</label><br>
                    <input type = "password" name="password">
                    <input type = "submit">
                </form>
            Checkbox
                <input type="checkbox" name = "dog" value = "Dog">
                <label for = "checkbox" name= "cat" value = "Cat">
            Radio button
                <input type = "radio" name = "right" value = "Right">
                <label for = "right"> I am right-handed</label><br>
                <input type = "radio" name = "left" value = "Left">
                <label for = "left"> I am left-handed</label><br>
            Other
                <input type = "number" name = "age">
                <input type = "email" name = "email">
                <input type = "file" name = "file">
            Textarea
                <input type = "text" name = "username">
                <textareaname = "multiline" rows = "5"></textarea>
            Drop-down list
                <select name = "food">
                    <option value = "chocolate">Chocolate</option>
                    <option value = "ice_cream">Ice Cream</option>
                </select>
    DOM
        Document Object Module
            Created when the browser receives an HTML to represent it
        Is
            A tree structure of the objects.
        Allows
            Dynamic modification of HTML components
        Contains
            Objects
                Following the hierarchy of HTML tags
    Web accesibility
        WAI
            Web Accesibility Initiative
        ARIA
            Accessible Rich Internet Application

### CSS
    Five elements
        Selector
            h1 {
                
            }
        Declaration
            Property
            Value
                color: grey;
    Linked to HTML
        At header tag
            <link rel = "stylesheet" href = "style.css">
    Selectors
            # -> id
            . -> class
        Element with selector
            Selecting all <p> with class "introduction"
                p.introduction {
                    property:value;
                }
        Descendent selectors
            Selecting all h1 elements inside element with ID blog
                #blog h1 {
                    property:value;
                }
            Various descendents
                Select h1 descending div descending blog
                    #blog div h1 {
                        color: blue;
                    }
            Secondary selectors
                Specific selection of only immediate descendant
                    #blog > h1 {
                        color: blue;
                    } 
            Psedoclasses
                Select based on the status
                    For example
                        :hover will change the a element when hover over it
                            a:hover {
                                color: orange;
                            }
    Declarations
        Color
            RGB
                color: rgb(255, 0, 0); 
            RGBA
                color: rgba(255, 0, 0, 128); 
            HSL
                Represented by a cilinder
                    Hue: 360 rotation
                    Saturation: From center (0%, white) to border (100%,black)
                    Lightness: From top (100%, white) to bottom (0%, black)
                        color: hsl(0, 100%, 50%);
            hexadecimal
            predefined color names
        Font
            font-family: "Courier New", monospace;
            font-size: 12px;
        Text transform and decoration
            text-transform: uppercase;
            text-decoration-line: underline;
            text-decoration-color: red;
            text-decoration-style: solid;
            text-decoration-thickness: 5px;
    Box Model
        4 parts
            Margin
                Extends the border area to separate from neighboring elements
                    Box size
                        Border Box width + margin left-side + margin right-side
                        Same with respective for height 
                    Size
                        margin-top:4px;
                        margin-bottom:4px;
                        margin-left:4px;
                        margin-right:4px;
            Border
                Goes around the padding and content
                    border-width:thin,medium,thick;
                Size
                    Padding with + border left and right sides
                    Same with respective for height
                Types
                    Solid
                    Dashed
                    Dotted
                    Double
            Padding
                Extends the content size
                    Size
                        thickness
                            padding-top:4px;
                            padding-bottom:4px;
                            padding-left:4px;
                            padding-right:4px;
                        width
                            content width + padding left-side + padding right-side
                        height
                            content height + padding top-side + padding bottom-side
            Content
                Contains the actual content of elements
                    size and width
                        width:1px;
                        min-width:1px;
                        max-width:2px;
                        height:1px;
                        min-height:1px;
                        max-height:2px;
        Shorthand properties
            Another way to set size
                Padding:4px 2px 1px 5px;
                Border-Width:2px 3px 1px 4px;
                Margin:1px 2px 4px 5px;

