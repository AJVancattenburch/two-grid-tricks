# two-grid-tricks

Bootstrap Training Repo Information Located Below:

BACKGROUND & OBJECTIVES
Now that you are Bootstrap-grid experts, learn more advanced but very usefull techniques with the grid.

SPECS
99% of the time you face two issues using the grid:

You need a full-screen background around your grid.

You need to insert some kind of inner "cards" into your grid.

You should never change the width, border, and lateral paddings of the grid components (.container, .row or .col). Because if you do so, you will break the grid. So here is how you can do:

full-screen background: place a background div around the grid.

<div class="bg-blue">

  <div class="container-fluid">

    <div class="row">

      <!-- all you cols -->

    </div>

  </div>

</div>
.bg-blue {

  background: #3079AB;

  color: white;

}
inner "cards": place nice divs inside the col

<div class="container">

  <div class="row">

    <div class="col-12 col-md-6">

      <div class="card-white">

        <!-- card content -->

      </div>

    </div>

    <div class="col-12 col-md-6">

      <div class="card-white">

        <!-- card content -->

      </div>

    </div>

  </div>

</div>


.card-white {

  background: white;

  padding: 30px;

  box-shadow: 1px 1px 2px #e7e7e7;

  border-radius: 4px;

  margin: 20px 50px;

}
With these two techniques, you can put as much padding, border, margin as you want and you will never break the grid, since you never touch directly at grid components (container/row/col).

YOUR TURN
Apply these two techniques to reproduce this page

![Two Grid Tricks Challenge Image](url "two-grid.jpg")

 
Use the starting HTML and CSS from above as a starting point. You will have to code a bit of CSS for backgrounds, padding and margin.