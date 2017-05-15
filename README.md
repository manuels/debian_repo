[User] Install Software

    echo "deb https://manuels.github.io/debian_repo jessie main" | sudo tee /etc/apt/sources.list.d/manuels.github.list
    wget -qO - https://manuels.github.io/debian_repo/public.key | sudo apt-key add -
    sudo apt-get update
    sudo apt-get install bulletinboard # or whatever software you want

[Admin] Add new software

    reprepro -b . includedeb jessie myfile.deb
