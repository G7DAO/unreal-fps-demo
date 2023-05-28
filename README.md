# unreal-fps-demo

unreal-fps-demo uses [web3.unreal](https://github.com/G7DAO/web3.unreal) as a git submodule to demonstrate its functionality and for use in development

[<img alt="Discord" src="https://img.shields.io/discord/593655374469660673.svg?style=for-the-badge&label=Discord&logo=discord" height="20">](https://discord.gg/Vx4ky6ZbAK)
[<img alt="Twitter" src="https://img.shields.io/twitter/follow/espadrine.svg?style=for-the-badge&label=Twitter&color=1DA1F2" height="20">](https://twitter.com/HyperPlayGaming)

## Common Issues
* When switching branches with the FPS_Demo project, be sure to right click the .uproject and ensure the right engine version is selected with "Switch Unreal Engine Version...". 
  * You should also click "Generate Visual Studio Project Files" if they are not automatically generated after the last step. 
  * Then you must build through your editor. We recommend Visual Studio 2022 or JetBrains Rider. We don't recommend Visual Studio 2019 due to its performance, but it will work as well.

## Contributing
Follow these instructions to start contributing to web3.unreal:
* Clone the repo with 
```
git clone --recurse-submodules https://github.com/G7DAO/unreal-fps-demo.git
```
* Ensure that the web3.unreal submodule was cloned correctly
* Right click `FPS_Demo.uproject`, click `Switch Unreal Engine Version`, and select the engine version you would like to develop with
  * We have tested with UE 4.27 - 5.1
* Right click `FPS_Demo.uproject` and click `Generate Visual Studio Project Files`
* Open FPS_Demo.sln
* Select `Development Editor` as the build configuration
* Right click FPS_Demo in the solution explorer and select `Build`
* Launch `FPS_Demo.uproject`
* If you get a "Fetch is Incompatible" popup, click yes. 
  * We include the [Fetch plugin](https://github.com/GDi4K/unreal-fetch) as a separate option to Web3.Unreal for making 3rd party rpc calls, but it has restrictive commercial licensing (Creative Commons Non-Commercial license), error prone syntax, and lots of boilerplate. 
* In `Content/FirstPersonBP/Blueprints/FirstPersonCharacter`, there are many examples of web3 functionality that can be performed with web3.unreal
  * Check out the `Web3UnrealExamplesGraph` for a list of examples
* Get some goerli eth [here](https://goerlifaucet.com/)
* Play the game. Interacting with the items on the wall will request web3 transactions
  * You will need to have the HyperPlay desktop app running to perform this functionality. Sign up for early access [here](https://docs.google.com/forms/d/e/1FAIpQLSeBWkOkzUZ6K_i8f6181upDcOFPgGv-7A2KxsSgqUQTPz3h4Q/viewform). Otherwise you will only be able to use web3.unreal for 3rd party reads
    * HyperPlay will be fully open sourced in early 2023
  
Feel free to submit an issue or PR to web3.unreal if you cannot find the functionality that you need
