# Demo
This repository contains the source of the demo UE project that is shipped with Scalable Pixel Streaming.

## Installing the Unreal Engine

Follow the [official documentation](https://www.unrealengine.com/en-US/download) or access the [official repository](https://github.com/EpicGames) to download and install the Unreal Engine on your chosen platform. The project was built for UE version 5.0 or newer.

## Building the project

1. Launch the Unreal Editor.
2. Clone this repo `git clone https://github.com/ScalablePixelStreaming/Demo.git`.
3. Open the VehicleTouch50.uproject file in the editor. The project is already set up with Pixel Streaming plugin enabled.
4. Package the project for Linux, or Windows if your chosen cloud platform supports Windows containers. Refer to our documentation for more information on this step, especially since packaging for Windows requires additional preparation steps.
5. Once your project is packaged for target platform, you are ready to deploy it to your SPS formation.
6. If your cloud platform supports creating versions from a compressed UE project, create a `.zip` archive and upload it directly via the CLI tool or dashboard. Read more about this step here. Your application should now be ready to stream.
7. If your cloud platform doesn't support creating versions from a compressed UE project, use our Image Builder Tool to create a container image suitable for deploying on SPS. Read more about this step here.
8. Create a version using the newly created container tag. Read more about this step here. Your application should now be ready to stream.

Refer to our documentation for a more detailed look into Scalabel Streaming entities hierarchy and step-by-step deployment guides.

## Legal

Copyright &copy; 2021 - 2024, TensorWorks Pty Ltd. Licensed under the MIT License, see the file [LICENSE](./LICENSE) for details.
