# Generate fake test data for Magento

MageFaker is a tool for creating a bunch of bogus customer accounts, products and orders on a Magento installation using realistic, yet fake, customer data.

![image](http://up.nicksays.co.uk/image/0240281V1D1e/Screen%20Shot%202012-11-27%20at%2000.12.07.png)

### Installation

    git clone https://github.com/punkstar/magefaker.git ~/magefaker
    cd ~/magefaker
    composer install
    echo "alias magefaker=~/magefaker/bin/magefaker" >> ~/.zshrc

### Usage

Following command will create 1K fake products, 50K fake customer accounts, 3 fake orders (5 purchase items each) per customer & 20K fake guest orders for the Magento installation at `~/Sites/my/magento/root`.

    magefaker --magento ~/Sites/my/magento/root --products 1000 --customers 50000 3 5 --guestorders 20000