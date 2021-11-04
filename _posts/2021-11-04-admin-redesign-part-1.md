---
layout: post
author: kalju
---

<div class="section">
    <p>When planning the Nice Train Website documentation, I realized I didn't have an overarching theme or plan for the admin UI. I figured it was for my use only, so it wasn't necessary to really plan the layout or aesthetics. The result is something ugly and difficult to use (enough so that I kind of dread using it). There's also the fact that I made the admin side publicly visible, with the intention of demonstrating my front-end competence.
    </p>
    <div class="captioned-img">
        <span>not appealing, not particularly functional</span>
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/old_admin.jpg" alt="old admin example" title="vomit emoji"/>
    </div>
</div>

<div class="section">
    <p>
    I decided to start the admin redesign with a more detailed plan. The initial plan is to:
    </p>
    <ul>
        <li>use the 'train pamphlet' style</li>
        <li>use Grid Layout instead of Flexbox</li>
        <li>design mobile-first</li>
        <li>(try to) approach every element as an independent element</li>
        <li>translate as much of the design as I can into Grid Layout before starting to code</li>
    </ul>
</div>

<div class="section">
    <p>
    I started with the Scheduled Trains UI, and tried to plan out a manageable number of typography and shape variations.    
    </p>
    <div class="screen-plan-row">
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/scheduled_trains.jpg" alt="scheduled trains mockup"/>
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/scheduled_trains_type.jpg" alt="scheduled trains typography map">
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/scheduled_trains_shape.jpg" alt="scheduled trains shape map">
    </div>
</div>

<div class="section">
    <p>
    The tab-navigation works ok on desktop, but on mobile is a bit of a condensed mess.  I'm going to replace it with a drawer.
    </p>
    <div class="screen-plan-row">
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/nav_drawer.jpg" alt="nav drawer mockup"/>
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/nav_drawer_type.jpg" alt="nav drawer typography map">
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/nav_drawer_shape.jpg" alt="nav drawer shape map">
    </div>
</div>

<div class="section">
    <p>
    The activity list will expand to full-screen, and editing will be done with three dropdowns.
    </p>
    <div class="screen-plan-row">
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/editor_activities.jpg" alt="activity editor mockup"/>
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/editor_activities_type.jpg" alt="activity editor typography map">
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/editor_activities_shape.jpg" alt="activity editor shape map">
    </div>
</div>

<div class="section">
    <p>
        After laying these out I made a small shape-and-style guide, and adjusted any rogue shapes or type to conform with it.  Hopefully it's useful when making the rest of the admin UI.
    </p>
    <div class="captioned-img">
        <img class="mobile-screen" src="{{site.baseurl}}/assets/images/admin_redesign/shape_type_guide.jpg" alt="shape and type guide">
    </div>
</div>

<div class="section">
    <p>
        My plan is to implement these before mocking up the rest of the admin UI, as there will probably be something I want to change about the design-n-mock process.
    </p>
</div>
