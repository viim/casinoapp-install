# casinoapp-install
Install script for CASinoApp without user interaction. CASinoApp is a ready to use implementation for a CAS (Central Authentification Service) server available here: [https://github.com/rbCAS/CASinoApp](https://github.com/rbCAS/CASinoApp).

Installation of CASinoApp requires running the `script/install` script, which interacts with the user. In our case, we make an automated install of CASinoApp, so we need two non-interacting scripts which can be found here.

In order to use this scripts, download the CASinoApp, and instead of running `script/install`, simply do the following:

1. `git clone https://github.com/viim/casinoapp-install.git`
2. Run `casinoapp-install/install-step-1 <your-database>`. `<your-database>` can be postgres, mysql or sqlite
3. Edit the config files `config/database.yml` and `config/cas.yml` to fit your installation
4. Run `casinoapp-install/install-step-2`

