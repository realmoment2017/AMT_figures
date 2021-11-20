<!-- You must include this JavaScript file -->
<script src="https://assets.crowd.aws/crowd-html-elements.js"></script>

<!-- For the full list of available Crowd HTML Elements and their input/output documentation,
      please refer to https://docs.aws.amazon.com/sagemaker/latest/dg/sms-ui-template-reference.html -->

<!-- You must include crowd-form so that your task submits answers to MTurk -->
<crowd-form answer-format="flatten-objects">

  <crowd-instructions link-text="View instructions" link-type="button">
    <short-summary>
      <p>We are providing pair of images and asking about the opinions about them.  Please rate the folowing pictures according to structural similarity and textural similarity.</p>
    </short-summary>

    <!--<detailed-instructions>-->
    <!--  <h3>Provide more detailed instructions here</h3>-->
    <!--  <p>Include additional information</p>-->
    <!--</detailed-instructions>-->

    <!--<positive-example>-->
    <!--  <p>Provide an example of a good answer here</p>-->
    <!--  <p>Explain why it's a good answer</p>-->
    <!--</positive-example>-->

    <!--<negative-example>-->
    <!--  <p>Provide an example of a bad answer here</p>-->
    <!--  <p>Explain why it's a bad answer</p>-->
    <!--</negative-example>-->
  </crowd-instructions>

  <!--<div>-->
  <!--  <p>What is your favorite color for a bird?</p>-->
  <!--  <crowd-input name="favoriteColor" placeholder="example: pink" required></crowd-input>-->
  <!--</div>-->

  <!--<div>-->
  <!--  <p>Check this box if you like birds</p>-->
  <!--  <crowd-checkbox name="likeBirds" checked="true" required></crowd-checkbox>-->
  <!--</div>-->
  
  <!--<iframe width="973" height="547" src="https://www.youtube.com/embed/bUbV2iQw2tk" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>-->
  <!--<iframe width="973" height="547" src="http://25.media.tumblr.com/12c5772ea9eb06d2df604c8ff42bc9f8/tumblr_moxcx9AWnN1s4obsuo1_500.gif" ></iframe>-->
  
  <div>
    <p>Is this pair of images similar in terms of structure (e.g., identity, layout, etc)? (not considering the background)
    
    1. Strongly disagree 
    2. Disagree 
    3. Neither agree or disagree 
    4. Agree 
    5. Strongly agree</p>
  </div>
  <div>
      <img src="${CoordGAN_swap_texture}" />
  </div>
  
  
  <div>
    <p>Is this pair of images similar in terms of structure (e.g., identity, layout, etc)?  (not considering the background)
    
    1. Strongly disagree 
    2. Disagree 
    3. Neither agree or disagree 
    4. Agree 
    5. Strongly agree</p>
  </div>
  <div>
      <img src="${DiagonalGAN_swap_texture}" />
  </div>
  
    <div>
    <p>Is this pair of images similar in terms of texture (e.g., face/hair color, lighting, etc)? (not considering the background)
    
    1. Strongly disagree 
    2. Disagree 
    3. Neither agree or disagree 
    4. Agree 
    5. Strongly agree</p>
  </div>
  <div>
      <img src="${CoordGAN_swap_structure}" />
  </div>
  
  <div>
    <p>Is this pair of images similar in terms of texture (e.g., face/hair color, lighting, etc)?  (not considering the background)
    
    1. Strongly disagree 
    2. Disagree 
    3. Neither agree or disagree 
    4. Agree 
    5. Strongly agree</p>
  </div>
  <div>
      <img src="${DiagonalGAN_swap_structure}" />
  </div>
  

  <!--<div>-->
  <!--  <p>Write a short essay describing your favorite bird</p>-->
  <!--  <crowd-text-area name="essay" rows="4" placeholder="Lorem ipsum..." required></crowd-text-area>-->
  <!--</div>-->
</crowd-form>
