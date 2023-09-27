# kxss
[1.1]: http://i.imgur.com/tXSoThF.png
[1]: https://twitter.com/TobiunddasMoe
This a adaption of tomnomnom's kxss tool with a different output format. I didn't want to fork his whole Hacks-Repository so created my Own ;-)

All Credit for this Code goes to [Tomnomnom](https://github.com/tomnomnom/)

## Changes to original kxss
I changed the output format of kxss to make it better grepable for my recon script. My new Output Looks like this:
```
URL: https://www.**********.***/event_register.php?event=177 Param: event Unfiltered: [" ' < >]
```

## Installation
To install this Tool please use the following Command:
```
go get github.com/Emoe/kxss
# or
go install -v github.com/Emoe/kxss@latest
# or
git clone https://github.com/Emoe/kxss.git
cd kxss/
go build main.go
mv main kxss
cp kxss /usr/local/bin/kxss
```

## Usage
To run this script use the following command:
```
echo "https://www.**********.***/event_register.php?event=177" | kxss
# or
echo "http://testasp.vulnweb.com/Search.asp?tfSearch=ok" | kxss
```

## Question
If you have an question you can create an Issue or ping me on [![alt text][1.1]][1]
