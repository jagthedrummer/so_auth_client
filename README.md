## SoAuthClient

This is a small app to demonstrate how to use the
[so_auth](https://github.com/jagthedrummer/so_auth) gem to delegate
authentication to the
[so_auth_provider](https://github.com/jagthedrummer/so_auth_provider).

Copy the `sample.env` file to `.env`.

To run this project locally you'll also want to run [so_auth_provider](https://github.com/jagthedrummer/so_auth_provider).

Once so_auth_provider is running you should visit `/oauth/applications`
(probably http://localhost:3000/oauth/applications).  Then click on "New Application",
then enter a name, and the callback URL that the client will be using
(probably http://localhost:3001/auth/so/callback).  Then copy the
Application ID and Secret into your `.env` file.

Then to start the app you can run `foreman start`.  (BTW, you may need
to install foreman with `gem install foreman`.)

See [http://www.octolabs.com/so-auth](http://www.octolabs.com/so-auth)
for more details.

