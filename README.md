# sample-same-domain-cookie-issue

To reproduce the issue, first start the application: `docker compose up`

Then, open the browser and navigate to http://localhost:8080/. You should see:

> The feature flag "test" is disabled!


Then open unleash at http://localhost:8080/unleash/ and sign in with admin/unleash4all.

If you go back to the initial page, you should see:

> waiting for feature flag "test" status

If you go back to the unleash UI and close the session, the problem in the home page will be solved.