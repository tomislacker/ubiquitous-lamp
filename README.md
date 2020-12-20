# Budget Gamer
_For when you're too damn cheap to build a gaming rig..._

## About
This project started with a few friends and colleagues riding me to play a
a couple different games with them. Given that I don't game much, I wanted
to see about using my [AWS] skills to be able to play periodically, with
reasonably high graphics, but without having to make a capital expenditure.

### Initial Experiment
* `g4dn.2xlarge` [EC2] with 100GB of `gp2` [EBS]
    * Running as a [Spot] instance
    * Using [NVIDIA Gaming PC - Windows Server 2019] image
* Streaming via [Parsec]
* Ran approximately 5.5hrs, playing about 4hrs, used about $0.012 in outbound
bandwidth

#### Initial References
* [parsec-cloud/Parsec-Cloud-Preparation-Tool]
* [forums.developer.nvidia.com/t/password-not-available-yet-aws-windows/112215]
* [Richard Neil Ilagan - How to: Create a Remote Gaming Server using Parsec on AWS]
* [TensorIoT Editor - Cloud Gaming on Amazon Web Services]
* [@mlabouardy - How to play PUBG on AWS]

## Roadmap
* Automation for:
    * Bootstrapping an [EC2] instance
    * Patching a previously bootstrapped instance
    * Starting/stopping the game
    * Ensuring an instance is not running idly
* Documentation for:
    * Getting started in AWS
    * Using this project

[AWS]: https://aws.amazon.com/what-is-aws/ "[aws.amazon.com] Amazon Web Services (AWS) is the world’s most comprehensive and broadly adopted cloud platform, offering over 175 fully featured services from data centers globally. Millions of customers—including the fastest-growing startups, largest enterprises, and leading government agencies—are using AWS to lower costs, become more agile, and innovate faster."
[EBS]: https://aws.amazon.com/ebs/ "[aws.amazon.com] Amazon Elastic Block Store - Easy to use, high performance block storage at any scale"
[EC2]: https://aws.amazon.com/ec2/ "[aws.amazon.com] Amazon EC2 - Secure and resizable compute capacity to support virtually any workload"
[NVIDIA Gaming PC - Windows Server 2019]: https://aws.amazon.com/marketplace/pp/B07STLTHM8 "[aws.amazon.com] NVIDIA Gaming PC - Windows Server 2019 - GPU-Accelerated Cloud Gaming"
[Parsec]: https://parsec.app/ "[parsec.app] Parsec connects you to your work, games, and friends wherever you are, across any device in crystal clear, interactive HD."
[Richard Neil Ilagan - How to: Create a Remote Gaming Server using Parsec on AWS]: https://www.richardneililagan.com/posts/create-game-server-aws-parsec "[richardneililagan.com] How to: Create a Remote Gaming Server using Parsec on AWS"
[Spot]: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/spot-fleet-requests.html "[docs.aws.amazon.com] Amazon Elastic Compute Cloud - Spot Fleet requests"
[forums.developer.nvidia.com/t/password-not-available-yet-aws-windows/112215]: https://forums.developer.nvidia.com/t/password-not-available-yet-aws-windows/112215 "[forums.developer.nvidia.com] Password not available yet AWS windows."
[parsec-cloud/Parsec-Cloud-Preparation-Tool]: https://github.com/parsec-cloud/Parsec-Cloud-Preparation-Tool "[github.com] parsec-cloud/Parsec-Cloud-Preparation-Tool"
[TensorIoT Editor - Cloud Gaming on Amazon Web Services]: https://medium.com/tensoriot/cloud-gaming-on-amazon-web-services-4be806c0051b "[medium.com] TensorIoT Editor - Cloud Gaming on Amazon Web Services"
[@mlabouardy - How to play PUBG on AWS]: https://hackernoon.com/how-to-play-pubg-on-aws-db2e75fa599b "[hackernoon.com] @mlabouardy - How to play PUBG on AWS"
