<h1>This project is for learning spring security</h1>
<div>
    <label>Things to cover : </label>
    <ol>
        <li>Authentication.</li>
        <li>Authorization.</li>
        <li>Filter Chain.</li>
    </ol>
</div>

<ol>
    <li><h4>Authentication : </h4>
        <ul>
            <li>Authentication is nothing but proving an identity, i.e. lets
            say that MR X wants to login to a website,he has to prove he is MR X
            , so how? by providing password, or biometric data etc. Now he proves and gets authenticated.
            </li>
        </ul>
    </li>
    <li><h4>Authorization : </h4>
        <ul>
            <li>Now MR x has proved his identity, but he wants to access some data, is he allowed to 
                access the particular data, so this is authorization.
            </li>
            </br>
            <li>
               A real world example is in a company we have three level of security to a building, 
                one is till reception, next is into office area, next is into server room, Now a CEO will have 
                all 3 security clearance, whereas a normal employee will not have authority to enter into
                the server rooms, so this is authorization. CEO -> has 3 level security clearance
                whereas the employee -> only two levels of security clearance.
            </li>
        </ul>
    </li>
    <li><h4>FilterChain : </h4>
        <ul>
            <li>
                They are series of filter a request goes through when they reach the server,
                to check the authentication and authorization of the request.
            </li>
            <br>
            <li>
            Spring provides default configuration of security chain when Spring Security pacakge
            is used, it can be overridden and also highly customizable.
            </li>
        </ul>
    </li>
</ol>
<h3>Spring Security Architecture (src : miro.medium.com) : </h3>
<img src="https://miro.medium.com/v2/resize:fit:932/1*66qT-P8eO7psafi_t5jfcA.jpeg">

<h5>Default Security Filter Configuration : </h5>
<ul>
    <li><b>SpringBootWebSecurityConfiguration</b> is the class that provides 
        default web security configuration for spring boot applications.</li>
    <li>This can be overridden by our own custom security configuration</li>
</ul>