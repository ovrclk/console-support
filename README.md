# Overclock Console Support Page

Thank you for using Akash Console!

If you have issues to report or features to request,
please enter them [here](https://github.com/ovrclk/console-support/issues/new/choose).

When reporting an issue, please take care to be as thorough as possible.  The easier
it is for us to reproduce an issue, the faster we can address it!

Your feedback is greatly appreciated; we'll be addressing issues and evaluating
suggestions on an ongoing basis.


# What to test

Anything is fair game but to provide some guidance, here are areas worth touching on:

1. Certificate management: <br>
   a. Should be able to create a certificate from the settings page and from the "checking essentials" page (the "preflight-check" page).<br>
   b. Should be able to revoke a certificate that was created with Console from the settings page.<p>
2. Wallet connection: <br>
   a. Should only prompt you to login to your wallet when you get to the "checking essentials" (pre-flight check) page and only if you are not logged into your keplr wallet.<br>
   b. Should check wallet connection AND funds (5AKT) during the pre-flight check.<br>
   c. Should be able to switch between multiple wallets and have the various screens (settings/ certs, preflight check, deployments list) reflect the state based on the active wallet.<p>
3. Deployment List:<br>
   a. Should be able to view ALL deployments made using a wallet (regardless of whether they were made with Console or a different tool). The count of the deployments, the order (sorted by DSEQ, descending) and the pagination should work as expected.<br>
   b. Should be able to toggle between just active and both active and inactive deployments.<br>
   c. Should be able to click it and see details of each deployment.<p>
4. Deployment workflow:<br>
   a. Verifying the full cycle: Deploy -> Confirm deployment -> View Deployment in List -> Update Deployment -> Confirm update -> Delete Deployment -> Confirm inactive.<br>8
   b. Should be able to deploy using both pre-defined templates and the "Import SDL" function (where you can deploy with any custom SDL). *NOTE* that some of the omnibus templates that power the RPC nodes may be in a bad state but the deployment via Console should suceed. In this case, confirming that the events and logs show up in Console (even if the logs indicate a bad polkachu snapshot or something) is sufficient to test Console deploy.<br>
   c. For each case, changing/ modifying the configuration via the UI (by clicking into each service in the parameter editor page) should reflect the changed state in the raw SDL editor ("Edit SDL" button).<br>
   d. App should handle update deployment and re-deployment workflows.<br>
   e. Lease details should look accurate.<br>
   f. Should be able to add additional funds to youu deployment escrow from the deployment details page.<br>
   
