# Locale en_CH

Sources : 
 - https://askubuntu.com/a/162714/868786
 - https://lh.2xlibre.net/locale/en_US/
 - https://lh.2xlibre.net/locale/fr_CH/

# Installation

_tested on Ubuntu 18.10_


	wget https://raw.githubusercontent.com/cbaconnier/ubuntu-locale-en_CH/master/en_CH
	sudo localedef -i en_CH -f UTF-8 en_CH.UTF-8 -c -v
	sudo mv en_CH /usr/share/i18n/locales/
	echo 'en_CH UTF-8' | sudo tee --append /var/lib/locales/supported.d/en
	sudo locale-gen
	
	
 - Change the regional settings with the new locale in `Language Support` > `Regional Formats` and search for `Switzerland (English)`

Next time you log in, the locale should be in use.
