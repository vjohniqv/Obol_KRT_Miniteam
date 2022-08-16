# Obol_KRT_Miniteam
Obol_KRT_Miniteam --> 201/200 😆😆😆 - our team notes.

Obol Athena Testnet
-------------------
Guide: [Lets Node - Obol](https://teletype.in/@letskynode/obol_athena_testnet) ; Google Sheet: [Athena Validator](https://docs.google.com/spreadsheets/d/1Zr0jx2ROxe2db2Geu79BDR7BDlKonB3qKzBprqEW_Ao/edit#gid=0) ; Explorer: [Goerli.Beaconcha](https://goerli.beaconcha.in/validator/0xa8623551ba27e8e5e5f57775806316ef5091448a4d20c86be6244baf2d964a912dd527e3265927f9b9521997e67baa02#deposits) .

KRT_Miniteam
------------
`Role` | `Name` | `Nickname` | `Discord` | `Grafana`
--- | --- | --- | --- | ---
Captain | Merlin | wild-soup | [Mutant#6520](https://discord.com/users/877965122595868722) | [Merlin](http://178.150.62.251:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | Leypx | bountiful-death | [LEYPX#7886](https://discord.com/users/401855964745302046) | [Leypx](http://135.181.92.161:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | R | innocent-law | [Anatoliy#9670](https://discord.com/users/883017726661120001) | [R](http://65.109.28.243:3000/d/singlenode/single-charon-node-dashboard?orgId=1&from=now-30m&to=now&refresh=10s)
Member | Alex | bewildered-picture | [thealex11x#4706](https://discord.com/users/824364194580529172) | [Alex](http://94.158.152.162:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | My event Horizon | combative-boy | [ElectricWizard#9657](https://discord.com/users/194132632496373760) | [My event Horizon](http://142.132.151.169:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=5s)
Member | Zhenya | courageous-tea | [Johniq#8079](https://discord.com/users/304260322699640833) | [Zhenya](http://144.91.69.106:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | Dmitrii | black-pen | [Fuckermaker ClayClan#2082](https://discord.com/users/867052848735191070) | [Dmitrii](http://144.76.118.94:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | Maks | wise-rate | [Maksimoos#0207](https://discord.com/users/598959147794563081) | [Maks](http://142.132.149.221:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)

Node update
-----------
To update to the latest version use this command:
```
cd ~/charon-distributed-validator-node/ && docker-compose down && git pull && docker-compose up -d
```
If something went wrong and an error occurred, try resetting the version and downloading it again:
```
cd ~/charon-distributed-validator-node/ && docker-compose down && git reset --hard HEAD && git pull && docker-compose up -d
```
That`s all.

Usefull Commands
----------------
Check all logs
```
cd ~/charon-distributed-validator-node && docker-compose logs --tail=100 -f
```
Check attestation logs
```
cd ~/charon-distributed-validator-node && docker logs charon-distributed-validator-node-charon-1 --tail=100 -f
```
Check current epoch
```
cd ~/charon-distributed-validator-node && docker-compose logs --tail=100 -f | grep 'epoch: '
```
Restart
```
cd ~/charon-distributed-validator-node/ && docker-compose down && docker-compose up -d
```
Stop
```
cd ~/charon-distributed-validator-node/ && docker-compose down
```
Start
```
cd ~/charon-distributed-validator-node/ && docker-compose up -d
```
Put the same region
```
sudo timedatectl set-timezone Europe/Kiev
```

Our bootnode
------------
Edit our file to add bootnode:
```
nano ~/charon-distributed-validator-node/docker-compose.yml
```
Find the line: _*CHARON_P2P_EXTERNAL_HOSTNAME: charon*_ - and paste the text below it:
```
CHARON_P2P_BOOTNODES: http://38.242.247.35:3640/enr
```
After we press: _*Ctrl+O --> Enter --> Ctrl+X*_ - and restart your node:
```
cd ~/charon-distributed-validator-node/ && docker-compose down && docker-compose up -d
```
That`s all.

Obol links
----------
#### WebSite: [Obol.tech](https://obol.tech/) ; Discord: [Obol Network](https://discord.com/invite/n6ebKsX46w) ; GitHub: [Obol Network](https://github.com/ObolNetwork) ; Twitter: [Obol Labs](https://twitter.com/ObolNetwork) ; Docs: [Obol docs](https://docs.obol.tech/) ; Mail: support@obol.tech .
