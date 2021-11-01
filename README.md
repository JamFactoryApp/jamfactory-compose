# jamfactory-compose

## Development setup

* Clone the repository to your desired location
  ```sh
  git clone https://github.com/JamFactoryApp/jamfactory-compose.git
  ```
  
* If not already: Clone the following repositories to your desired location
  * JamFactoryApp/jamfactory-backend ``git clone https://github.com/JamFactoryApp/jamfactory-backend.git``
  * JamFactoryApp/jamfactory-web ``git clone https://github.com/JamFactoryApp/jamfactory-web.git``
  * JamFactoryApp/jamfactory-static ``git clone https://github.com/JamFactoryApp/jamfactory-static.git``

* Create a Spotify App on the [Developer Dashboard](https://developer.spotify.com/dashboard)

* Create a ``.env`` file and fill out the information. See [.env.example](./jamfactory_dev/.env.example) for an example ``.env`` file.

* Create a ``users.acl`` file in the ``jamfactory_dev/redis`` folder. Make sure to use the same password as in the ``.env`` file.
  See [users.acl.example](jamfactory_dev/users.acl.example) for an example ``users.acl`` file.

* Create and start the development containers using ``docker-compose up -d``

* After successful startup, the JamFactoryApp is available under ``http://localhost``. Automatic reloading on code changes inside the JamFactoryApp/jamfactory-web and JamFactoryApp/jamfactory-static is supported.