# configure-mullvad-cli
Configure mullvad VPN headless/CLI only

1. Download and install the latest version https://mullvad.net/en/download/vpn/linux
2. Follow the basic guide on configuring your account https://mullvad.net/en/help/how-use-mullvad-cli
   1. `mullvad account login 1234123412341234`
   2. `mullvad account get`
   3. `mullvad relay list`
   4. `mullvad relay set location XX YY`
3. BEFORE running `mullvad connect`, run: `mullvad lan set allow` (https://mullvad.net/en/help/how-use-mullvad-cli : "Enable LAN access")
4. Connect `mullvad connect`
5. Verify `mullvad status -v`
6. Enable lockdown mode `mullvad lockdown-mode set on` (https://mullvad.net/en/help/using-mullvad-vpn-app#faq)
