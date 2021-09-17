# My Ideal Terminal

## Why?

A: well the reason I am posting this to maybe help others make their ideal terminal

## `.bashrc` Breakdown

- most of what is written down has comments explaining it so im just gonna explain some of it

- Aliases (starting at line #152 )
	- `h` is just a easy way of accessing the history
	- `bashrcEdit` was easier for me to remember than `nano ~/.bashrc` so its just a quick way of editing my `.bashrc`
	- [exa] is a modern version of the `ls` command. The `ls` alias is just how I like it by default. The alias `la` shows all files including hidden and 'dot' files. `lsa` lists the files and their permissions along with several other pieces of info. `lt` list the files as a tree format which can be helpful when dealing with folders
	- [lsd] lsd is what I used to use but found it not as good as exa so switched over but incase I ever descide to switch back I keep it in there
	- [batcat] is a alternative to cat that has syntax highlighting and has Git integration
	- `usb` allows me to quick way to do `source ~/.bashrc` since I used to not remeber it
	- `update-system` is a alias provided by a friend to update my package managers pretty easily
	- All the `...` commands do is allow me to go back a couple directories at the same time which 

- The `extract` function allows me to extract any compressed file I've needed to in the past and for some who doesnt automatically create a folder to extract it to it creates a folder for it
- for my prompt I use the [starship] bash prompt (you can find that config and a explation also in this repository) which is why i have `eval "$(starship init bash)"` in my `.bashrc`
- Bash can do auto-completion and can even do syntax-aware completion. This is done using the Bash Line Editor ([ble.sh]) and work very well for me

## `.starship.toml` Breakdown

Theres only a couple options that I changed
 - I added a new line between lines: `add_newline = true`
 - I have the success symbol changed to a symbol simmilar to a `>`
 - For my username I have my username in white unless in root where its black and the @ symbol in yellow and the directory in light blue
 - More information about configuring your `starship.toml` can be found [here](https://starship.rs/config/)



[exa]: https://github.com/ogham/exa
[lsd]: https://github.com/Peltoche/lsd
[batcat]: https://github.com/sharkdp/bat
[starship]: https://starship.rs
[ble.sh]: https://github.com/akinomyoga/ble.sh