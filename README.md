# Coinbase Stop Loss Bot

This bot will monitor the sell price on Coinbase and sell all your BTC if the
price falls below the set threshold. The script is intentionally not fancy or
featureful. It should be easy to see that it does the right thing, and
hopefully that reduces avenues for failure when it's trying to dump all your
BTC.

## Instructions

1. Configure settings in `coinbase-stop-loss.php`.
2. `./run.sh` in a tmux or screen session.
3. Sleep at night.

## More Info

You need to enable API access in your Coinbase account. It's disabled by
default. When you run the bot, it will prompt you for the API key in a password
field to keep it out of your shell history.

The stop loss threshold price, price check frequency, and notification
recipients are configurable in the first few lines of the PHP script. Please
set these to your liking *before* running it.

**I cannot be held accountable if this bot explodes and sells off your life
savings for a pittance. Use at your own risk.**

## License

Released under the MIT license.
