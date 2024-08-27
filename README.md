# Demo

This repository contains the source code of the UE vehicle template project that is shipped and deployed as a demo on every new SPS installation by defult. 

When your SPS installation is complete, the project will be ready for users to start spinning up application instances by following the demo application URL.

If you have opted not to install the demo during stack creation or deleted the project and want it back, follow the steps below to re-deploy it. Since it is a regular blueprint UE project, the deployment process is the same as it would be for any UE project, which you can follow fully in [our documentation](https://docs.scalablestreaming.io/getting-started).

## Installing the Unreal Engine

Follow the [official documentation](https://www.unrealengine.com/en-US/download) or access the [official repository](https://github.com/EpicGames) to download and install the Unreal Engine on your chosen platform. The demo project is compatible with UE version 5.0 or newer.

## Building the project

1. Launch the Unreal Editor.
2. Clone this repo `git clone https://github.com/ScalablePixelStreaming/Demo.git`.
3. Open the VehicleTouch50.uproject file in the editor. The project is already set up with the Pixel Streaming plugin enabled.
4. If your target platform is Linux, the project is ready for packaging out of the box. Follow the steps in the [official UE documentation](https://dev.epicgames.com/documentation/en-us/unreal-engine/packaging-unreal-engine-projects?application_version=5.3) to package the project.
5. If your target is Windows and your chosen cloud platform supports Windows containers, refer to [our documentation](https://docs.scalablestreaming.io/) for detailed information on preparing your Windows UE project, as there are additional mandatory steps.
6. Once your project is packaged for your target platform, you are ready to deploy it to your SPS formation.
7. If your cloud platform supports creating versions from a compressed UE project, create a `.zip` archive and [upload it directly via the CLI tool or dashboard](
https://docs.scalablestreaming.io/getting-started/deploying).
8. If your cloud platform doesn't support creating versions from a compressed UE project, use our Image Builder Tool to [create a container image suitable for deploying on SPS](
https://docs.scalablestreaming.io/getting-started/building-container).
9. [Create a version](https://docs.scalablestreaming.io/getting-started/deploying) using the newly created container tag. Your application should now be ready to stream.

Refer to our documentation for a more detailed look into Scalable Streaming entities hierarchy and step-by-step deployment guides.

## Legal

Copyright &copy; 2021 - 2024, TensorWorks Pty Ltd. Licensed under the MIT License, see the file [LICENSE](./LICENSE) for details.
