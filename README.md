# jQuery Cycle Image On Hover

**[See a demo](https://jeremyblaze.github.io/jQuery-Cycle-Image-Hover/)** • By [Jeremy Blaze](https://jeremyblaze.com/?ref=jquerycycleimage)

### Step 1. Install
```
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="jquery.cycleImages.js"></script>
```

### Step 2. Set up HTML
(Add as many of these to the page as you like)
```
<div class="hoverimg">
    <div class="cover">
        <img src="example-images/marathon/1.png">
    </div>
    <div class="gallery" style="display:none">
        <img src="example-images/marathon/1.png">
        <img src="example-images/marathon/2.png">
        <img src="example-images/marathon/3.png">
        <img src="example-images/marathon/4.png">
        <img src="example-images/marathon/5.png">
    </div>
</div>
```

### Step 3. Initialize
```
<script type="text/javascript">

    $(document).ready(function(){
        $('.hoverimg').each(function(){
            $(this).cycleImages({
                cover: $(this).find('.cover'),
                gallery: $(this).find('.gallery'),
                interval: 280
            });
        });
    });

</script>
```