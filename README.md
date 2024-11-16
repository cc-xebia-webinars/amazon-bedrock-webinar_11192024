# Integrating Generative AI Models into Your Apps with Amazon Bedrock

![Xebia Logo](https://imagedelivery.net/VKawrzTPdVOU6XYN26Rvmg/80a8db15-9456-4922-1fb5-ccfaa2e30500/public "Xebia Logo")

We’re not your usual experts. We are rebellious game-changers and professional knowledge-sharers. And quite fun, if we say so ourselves. Invest in your personal learning journey or upskill your entire organization by learning the tech skills of the future. Learn today to get ready for tomorrow!

[Learn More >>>](https://xebia.com/academy)

## Webinar Slides

[Download Slides](./docs/slides.pdf)

## Getting Started

To code with the instructor, create a fork of this repository, then create a GitHub Codespace on the fork. The Fork button is in the upper-right-hand corner of this page. Once forked, create the green Code button on your forked version to access the ability to create a Codespace.

GitHub provides a generous amount of free time for Codespaces each month (currently, 120 hours). You are responsible for any charges incurred if you exceed the free time. You can monitor your usage in the GitHub settings.

The AWS Bedrock Python demos are located in the `demos` folder. To run the demos, a virtual environment will need to be created.

1. Open a terminal window, and log into AWS with the AWS CLI.

  ```bash
  aws configure sso
  ```

  After answering a few question, a web browser will open.  After logging in through the web browser, it will attempt to redirect to `localhost:SOME_PORT` or `127.0.0.1:SOME_PORT`. This will `localhost` URL not work. Click on the `PORTS` tab, and update the `localhost` URL with the URL to the GitHub Codespace container and complete logging in.

1. In Visual Studio Code, open the `intro_to_bedrock.ipynb` in the `demos/aistylist` folder. In the upper right corner of the notebook, select a kernel. To create a new kernel, create a new virtual environment. The path to the Python interpreter is `/usr/bin/python`.

1. Follow the instructions in the `intro_to_bedrock.ipynb` notebook to configure the environment.

1. You are now ready to work through the lab exercise in the `aistylist.ipynb` notebook located in the `demos/aistylist` folder.

Special thanks to Amazon for providing this excellent demonstration: [https://github.com/aws-samples/amazon-bedrock-aistylist-lab](https://github.com/aws-samples/amazon-bedrock-aistylist-lab)


## License

The content of this repository is made available under the following [license](LICENSE).

<br>
Course content and teaching is provided by:<br>

[![Cloud Contraptions Logo](https://imagedelivery.net/VKawrzTPdVOU6XYN26Rvmg/aff3f165-00ec-4130-83d3-7ff4744f7d00/h=40,sharpen=1 "Cloud Contraptions Logo")](https://www.cloudcontraptions.com)
