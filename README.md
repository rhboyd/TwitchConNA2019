# Maintaining and Upgrading Your Twitch Extension

## Introductions (15 min)

Twitch: So, what are you going to show us today?

Richard: quick recap of the parts of a Twitch Extension and how to use serverless to simplify development [3-5 minutes]

T: "I've heard a lot about this serverless movement, can you tell me why I'd use that instead of running a server in my broom closet?"

R: Standard serverless pitch with a focus on Twitch Streamers and Developers [5-10 min]

## Intro to Serverless (20 min)

T: "That sounds great, but can we peek under the hood and see how we would actually build something using serverless tools"

R: Create a new Twitch Extension from the the Twitch Dev Rig and highlight the two main parts identified earlier [10 min]

T: "okay, but none of this is serverless, right?"

R: Pull out part of the backend logic and create a lambda function to do the same [10 min]

## Serverless Focus (35 min)

T: "That's really cool! Can we do the same for the rest of the backend?"

R: Add the Auth feature to ensure only 'real' Twitch users are using the Extension [15 min]

T/R: We'll both be covering secrets management and how to safely store app secrets in AWS

R: Add DynamoDB as a persistent data store to keep track of the Color scheme from the sample app [10 min]

## CI/CD (45 min)

T: "You just made a bunch of changes and some of them didn't quite work the way you wanted them to, what happens if we were working on this while the Extension was being used by our friends?"

R: "I would have a very bad day" 
introduction to version control, testing, deployments, etc.... [10 minutes]

T: "That seems like a big leap from where we have everything on our laptop, to having it all stored in the cloud and properly controlled?"

R: "Right, let's walk through doing this migration." Create CodeCommit Repo [5 min], Create CodeBuild Project [10 min], Create CodePipeline [10 min].

T: It looks like it's all set up, let's deploy it and see what happens

R: Makes a change to the application that we know will break, break is caught during the CodeBuild step [10 min]

## Wrap-up
