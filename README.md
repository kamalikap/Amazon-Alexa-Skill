# Amazon-Alexa-Skill


First create an account at "https://developer.amazon.com/". Use the same username and password you used to create the aws account.

Next follow the steps to learn more about amazon Alexa.

1. Check the region to be North Virginia.

2. Go to Lambda, Create function
   * Select AWS Serverless Application on Repository.
   * Search for Alexa in search box.
   * Select "Alexa-skills-kit-nodejs-premium-facts-skill"
   * Click on the Github Url. You will need this later.
   * Go to Lambda and write the application name-"Alexa-skill"
   * Click Deploy

   * Note:- To delete this, first we have to go to Services-> Management and Governance-> Cloud Formation-> Click-> Actions-> Delete Stack

3. Go to lambda
   * click on the function you created and observe the alexa code.
   * Copy the Arn from upper right corner of the page 

4. Go to your Amazon Developer services account.
   * Click on Amazon Alexa
   *  Click on Amazon Alexa consoles
   * Click on Skills
   * Fill up the details if you havn't filled before
   *  Click on Alexa skill kit
   * Create Skill
   * Skill name- Polly-skill
   * Click Custom
   * Create Skill
   * Start from scratch
   * Choose

5. Go to github Url, then "en-US.json"
   * Copy the code

6. Go back to Alexa Developer console and click on "JSON Editor" in Build. Paste the code.
   * Change the "invocationName" in the code to " polly skill". You can only have three words and also it cannot contain any uppercase letter.
   * Click on Save Model
   * Click on EndPoint
   * Select AWS Lambda ARN
      * Copy the Arn from Lambda function and paste it into Default Region.
      * Click on Save End Points
   * Click on Intents
   * Click Build Model. This will take some time to build.
   * Go to Test in the header
       * Allow microphone
       * Click on OFF and change to Development
   * Go to Build
       * Click Invocation
       * copy the invocation name
    * Go to Test 
       * Type in the box next to English US " open polly skill"
       * Start Speaking with Alexa.

       * Click on "Voice and Tone", click "Learn more about supported SSML tags"
       		* Go to audio and copy the sudio link with "Car-Fu"
       		* Paste it in the alexa console editor and Select Play.
       		Leave the Speak and audio tags, and delete the text(black in color).
       		* Keep src but delete the link.


 7. Go to S3 in AWS console.
    * Click on poly.mp3 bucket, where you have saved your polly mp3 files
    * Select a recording and copy the Object Url. (The audio file cannot be longer than 240 sec).

8. Go to Alexa console and paste it into audio src. Click Play.

9. You can also go to the Amazon Alex app and speak to alexa from there.
