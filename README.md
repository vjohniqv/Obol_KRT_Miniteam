# Obol_KRT_Miniteam
Obol_KRT_Miniteam --> Bia Testnet

Obol Bia Testnet
-------------------
Explorer: [Goerli.Beaconcha](https://goerli.beaconcha.in/validator/0x880bdc66b6baa7189610f753b90df476e0e9c032523ba17d0be89a5e9e92c6ec0b3279654c3ad897b857a15625bb3dd6#deposits) .

KRT_Miniteam
------------
`Role` | `Name` | `Nickname` | `Discord` | `Grafana`
--- | --- | --- | --- | ---
Captain | R | tough-ship | [ElectricWizard#9657](https://discord.com/users/194132632496373760) | [R](http://65.109.28.243:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | Merlin | adorable-soup | [Mutant#6520](https://discord.com/users/877965122595868722) | [Merlin](http://178.150.62.251:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | Leypx | tbd | [LEYPX#7886](https://discord.com/users/401855964745302046) | [Leypx](tbd)
Member | Alex | reliable rock | [thealex11x#4706](https://discord.com/users/824364194580529172) | [Alex](http://94.158.152.162:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | My event Horizon | clever-morning | [Anatoliy#9670](https://discord.com/users/883017726661120001) | [My event Horizon](http://65.109.112.11:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | Zhenya | wondrous-bulb | [Johniq#8079](https://discord.com/users/304260322699640833) | [Zhenya](http://95.217.144.113:3333/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | Dmitrii | bountiful-ring | [Fuckermaker ClayClan#2082](https://discord.com/users/867052848735191070) | [Dmitrii](http://65.109.58.243:3000/d/singlenode/single-charon-node-dashboard?orgId=1&refresh=10s)
Member | Maks | tbd | [Maksimoos#0207](https://discord.com/users/598959147794563081) | [Maks](tbd)
Member | Yuriy | tbd | [tbd](tbd) | [Yuriy](tbd)

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
Check sync progress
```
cd ~/charon-distributed-validator-node && docker-compose logs --tail=100 -f |grep progress
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

Obol links
----------
#### WebSite: [Obol.tech](https://obol.tech/) ; Discord: [Obol Network](https://discord.com/invite/n6ebKsX46w) ; GitHub: [Obol Network](https://github.com/ObolNetwork) ; Twitter: [Obol Labs](https://twitter.com/ObolNetwork) ; Docs: [Obol docs](https://docs.obol.tech/) ; Mail: support@obol.tech .
