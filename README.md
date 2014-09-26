Responsive Tooltips
=====================

Simple responsive jQuery tooltip.

1. [Requirements](#req)
2. [Setup](#deploy)
3. [Using the responsive tooltip](#global)
    * [General Use](#toolgeneral)
    * [Arrowed Use](#toolarrow)


## <a name="req"></a>Requirements

To use this tool tip you simply need to have jquery on your site, this is already set as a bower dependency.

## <a name="deploy"></a>Setup

### Option 1 - Bower -

    > bower install responsive-tooltip

### Option 2 - Using Git

    > git clone git@github.com:Moosylvania/Responsive-Tool-Tip.git

After your include for jQuery, then include responsive-tooltip.css and responsive-tooltip.js on your site.

## <a name="global"></a>Using the Responsive Tooltip

To use tooltips you have two options.  One which just displays with out any arrow at the top, and one that does.

#### <a name="toolgeneral"></a>For General Use -

Inside some wrapped element either a new div, p, li tag, etc - simply include a link with the class 'tooltip' on the page.  Right after that include a div with the content of that tooltip right after it with the class name tooltip.

Example -

    <li>
        On the <a href="#" class="tooltip">email order confirmation</a> you received after placing your order.
        <div class="tooltip">
            <h2>Email order confirmation</h2>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent porta bibendum ipsum, et dictum massa fringilla nec. Phasellus vel dignissim odio. Morbi posuere malesuada mollis. Sed placerat, purus quis fermentum ullamcorper, dolor lorem laoreet tellus, vitae feugiat augue urna vel justo. Vivamus eu dignissim velit, sed euismod ante. Nunc vitae imperdiet nibh. Donec ut tellus ac dui ultricies porta sit amet vitae lorem.
            </p>
        </div>
    </li>

In the above example when users click 'email order confirmation' it will then show that tooltip message in the div tag that is after the link.

#### <a name="toolarrow"></a> Arrow version of the tooltip.

To use an arrow tooltip just like before simply create a link with the class tooltip and a div with the class tooltip after it. The main difference is to add the class arrow to it.

Basic Arrow Example -


    <div class="content left">
        <a href="#" class="tooltip arrow">Learn more about the Rebate Visa Prepaid Card</a>
        <div class="tooltip">
            <h1>Terms &amp; Conditions</h1>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent porta bibendum ipsum, et dictum massa fringilla nec. Phasellus vel dignissim odio. Morbi posuere malesuada mollis. Sed placerat, purus quis fermentum ullamcorper, dolor lorem laoreet tellus, vitae feugiat augue urna vel justo. Vivamus eu dignissim velit, sed euismod ante. Nunc vitae imperdiet nibh. Donec ut tellus ac dui ultricies porta sit amet vitae lorem.
            </p>
            <p>
                Proin tellus mauris, elementum eget turpis et, sagittis feugiat tellus. Nunc venenatis at velit at vulputate. Nunc facilisis porta leo sit amet aliquet. Nullam aliquet sollicitudin sem, tincidunt ornare tortor aliquet congue. Morbi fermentum ante et lacinia dignissim. Phasellus sed vehicula libero, eu porttitor neque. Nunc nec elementum dolor. Ut dapibus, eros a ultricies vulputate, sapien urna semper odio, a auctor quam lacus quis ante. Sed rutrum at magna in laoreet. Proin dapibus mauris purus. Praesent et tellus in dui malesuada vehicula nec nec nisl. Sed fringilla dui ut orci egestas, non viverra neque luctus. Cras tristique a nulla nec bibendum.
            </p>
        </div>
    </div>

If for some reason you need to add more distance between the top of the tooltip and the content it is pointing to simply add in the class 'padded' to the tooltip link
