---
layout: posts
title: 'Day4 : Typos / corrections/ Developer Roadmap/ WakaTime Tracking'
---
# Day4: Typos and Corrections / Developer Roadmap / WakaTime Tracking

I wanted to tackle fixing some of my older posts. I don’t write the best so I wanted to scrub over what I already published and do some correcting. While I was working through some of this I realized that using git commands is starting to become second nature. I am going to tackle making some branches that will only target certain aspects of the [Jekyll](https://bit.ly/3dSoZTf) blog engine. These would be things like posts, pages, layouts, styling, and maybe some of the admin stuff.

I do this mainly to practice branching and merging >< I know for a fact that this is redundant and will only lead to more headaches and effort. But this is the path that I chose for myself.

## Developer Roadmap

A few years ago I came across the excellent [DevelopersRoadmap](https://bit.ly/2QztM2R) created by [Kamran Ahmad](https://bit.ly/32MKfTZ). The project has received a lot of praise from the development community and has since spawned a [YouTube](https://bit.ly/2QzKJtY) Channel with videos that follow the path established by the roadmap. I will be using this as my compass to tackle the Front-End roadmap over the new few months.
![](/assets/images/d4frontendmain.png):

## WakaTime

I have been using [WakaTime](https://bit.ly/3vmFUD0) for years now. WakaTime allows you to activly track code time in editors. I have seen the icon for VIM in the supported editors but since I have never used vim in the past I overlooked it. I found a great plugin that took some messing around with in order to get to work. I keep on forgetting that with Linux you NEED to read documentation and ask for help when needed. The problem that I was facing was staring at me the entire time essentially there was no WakaTime binary installed on my computer so there was no way for the plugin to ever get the informtion out to the dashboard. With great assistance from the [r/neovim subreddit](https://bit.ly/2QVnc6S) here is how I got WakaTime to work with NeoVim.

1 ``python3 -mpip install --user wakatime``
2 ``echo "Plugin 'wakatime/vim-wakatime'" >> ~/.vimrc && vim +PluginInstall``
3 restart vim 
4 ``:PlugInstall``
5 enter your API key and you are good to go!

![](/assets/images/d4wakadash.png)

I can run ``tail -f ~/.wakatime.log`` after enabling ``:WakaTimeDebugEnable`` from nvim for diagnostics as well. You can also find out how much time you have reported within 24 hours running ``:WakaTimeToday``
![](/assets/images/d4wakatimetoday.png)

I thought it would be fun to embed the data in the post and also on the main blog site for anyone interested in seeing the damage in the upcoming months. I am sure that the diversity of languages, enviroments and projects will grow.

That covers today :)
