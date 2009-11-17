!SLIDE 

## Teaching <font color="red">Ruby</font> To Kids
#####&nbsp;
#####Sarah Mei
#####&nbsp;
#####@sarahmei
#####sarahmei@gmail.com

!SLIDE 

## Expanding Young Minds With <font color="red">Ruby</font> 
#####&nbsp;
#####Sarah Mei
#####&nbsp;
#####@sarahmei
#####sarahmei@gmail.com

!SLIDE

## About me

!SLIDE

## GetSET

!SLIDE

<img src="img/shoes_logo.png">

!SLIDE

## Philosophy

!SLIDE

## Programming and Language

!SLIDE

## Setup

!SLIDE

<pre><code>
Shoes.app do

end
</code></pre>

!SLIDE

<img src='img/step0.png'>

!SLIDE

<pre><code>
Shoes.app do
  <span class='changedcode'>para "Hello, world"</span>
end
</code></pre>

!SLIDE

<img src='img/step1.png'>

!SLIDE

<pre><code>
Shoes.app do
  para "Hello, world"<span class='changedcode'>, :align => "center",
    :size => "xx-large"</span>
end
</code></pre>

!SLIDE

<img src='img/step2.png'>

!SLIDE

<pre><code>
Shoes.app <span class='changedcode'>:title => "My awesome application"</span> do
  para "Hello, world", :align => "center",
    :size => "xx-large"
end
</code></pre>

!SLIDE

<img src='img/step3.png'>

!SLIDE

<pre><code>
Shoes.app :title => "My awesome application" do
  <span class='changedcode'>background tomato</span>
  para "Hello, world", :align => "center",
    :size => "xx-large"
end
</code></pre>

!SLIDE

<img src='img/step4.png'>

!SLIDE

<pre><code>
Shoes.app :title => "My awesome application" do
  background tomato
  para "Hello, world", :align => "center",
    :size => "xx-large"<span class='changedcode'>,
    :stroke => saddlebrown</span>
end
</code></pre>

!SLIDE

<img src='img/step5.png'>

!SLIDE

<pre><code>
Shoes.app :title => "My awesome application" do
  <span class='changedcode'>def periwinkle
    rgb(180,170,205)
  end</span>
  background <span class='changedcode'>periwinkle</span>
  para "Hello, world", :align => "center",
    :size => "xx-large", 
    :stroke => saddlebrown
end
</code></pre>

!SLIDE

<img src='img/shoes-colors.jpg'>

!SLIDE

<img src='img/step6.png'>

!SLIDE

<pre><code>
Shoes.app :title => "My awesome application" do
  def periwinkle
    rgb(180,170,205)
  end
  background periwinkle

  <span class='changedcode'>button "Change the text" do
    @headline.text = "I'm changed!"
  end</span>

  <span class='changedcode'>@headline</span> = para "Hello, world",
    :align => "center", 
    :size => "xx-large", 
    :stroke => saddlebrown
end
</code></pre>

!SLIDE

<img src='img/step7.png'>

!SLIDE

<pre><code>
Shoes.app :title => "My awesome application" do
  def periwinkle
    rgb(180,170,205)
  end
  background periwinkle

  <span class='changedcode'>animate do 
    @button, @left, @top = self.mouse</span>
    @headline.text =
      <span class='changedcode'>"#{@button} #{@left} #{@top}"</span>
  end

  @headline = para "Hello, world",
    :align => "center", 
    :size => "xx-large", 
    :stroke => saddlebrown
end
</code></pre>

!SLIDE

<img src='img/step8.png'>

!SLIDE

<pre><code>
Shoes.app :title => "My awesome application" do
  def periwinkle
    rgb(180,170,205)
  end
  background periwinkle

  animate do 
    @button, @left, @top = self.mouse
    <span class='changedcode'>line 0, 0, @left, @top</span>
  end

  @headline = para "<span class='changedcode'>Draw!</span>",
    :align => "center", 
    :size => "xx-large", 
    :stroke => saddlebrown
end
</code></pre>

!SLIDE

<img src='img/step9.png'>

!SLIDE

<pre><code>
Shoes.app :title => "My awesome application" do
  def periwinkle
    rgb(180,170,205)
  end
  background periwinkle

  animate do 
    @button, @left, @top = self.mouse
    <span class='changedcode'>unless @button == 0
      line 0, 0, @left, @top
    end</span>
  end

  @headline = para "Draw!",
    :align => "center", 
    :size => "xx-large", 
    :stroke => saddlebrown
end
</code></pre>

!SLIDE

<img src='img/step10.png'>

!SLIDE

<pre><code>
Shoes.app :title => "My awesome application" do
  def periwinkle
    rgb(180,170,205)
  end
  background periwinkle

  animate do 
    <span class='changedcode'>previous_left = @left
    previous_top = @top</span>
    @button, @left, @top = self.mouse
    unless @button == 0
      line <span class='changedcode'>previous_left, previous_top,</span>
        @left, @top
    end
  end

  @headline = para "Draw!",
    :align => "center", 
    :size => "xx-large", 
    :stroke => saddlebrown
end
</code></pre>

!SLIDE

<img src='img/step11.png'>

!SLIDE

<pre><code>
  # ...
  animate do 
    # ...
  end

  <span class='changedcode'>button "Clear" do
    background periwinkle
    @headline.remove
    @headline = para "Draw!",
      :align => "center", 
      :size => "xx-large", 
      :stroke => saddlebrown
  end</span>

  @headline = para "Draw!",
    :align => "center", 
    :size => "xx-large", 
    :stroke => saddlebrown

end
</code></pre>

!SLIDE

<img src='img/step12.png'>

!SLIDE

### Why was it successful?
* ruby
* &nbsp;
* &nbsp;
* &nbsp;

!SLIDE

### Why was it successful?
* ruby - <font color="red">choose the right tools</font>
* &nbsp;
* &nbsp;
* &nbsp;

!SLIDE

### Why was it successful?
* ruby - <font color="red">choose the right tools</font>
* visual
* &nbsp;
* &nbsp;

!SLIDE

### Why was it successful?
* ruby - <font color="red">choose the right tools</font>
* visual - <font color="red">frequent deployment</font>
* &nbsp;
* &nbsp;

!SLIDE

### Why was it successful?
* ruby - <font color="red">choose the right tools</font>
* visual - <font color="red">frequent deployment</font>
* small steps
* &nbsp;

!SLIDE

### Why was it successful?
* ruby - <font color="red">choose the right tools</font>
* visual - <font color="red">frequent deployment</font>
* small steps - <font color="red">short iterations</font>
* &nbsp;

!SLIDE

### Why was it successful?
* ruby - <font color="red">choose the right tools</font>
* visual - <font color="red">frequent deployment</font>
* small steps - <font color="red">short iterations</font>
* flexible

!SLIDE

### Why was it successful?
* ruby - <font color="red">choose the right tools</font>
* visual - <font color="red">frequent deployment</font>
* small steps - <font color="red">short iterations</font>
* flexible - <font color="red">constant customer interaction</font>

!SLIDE

### Acknowledgements
##### &nbsp;
##### Screenshots - Satoshi Asakawa (@ashbb)
##### GetSET - www.getset.org
##### RailsBridge - teachingkids.railsbridge.org
##### Slidedown - Pat Nakajima (@nakajima)

!SLIDE

### Thank you!
##### &nbsp;
##### sarahmei@gmail.com
##### @sarahmei