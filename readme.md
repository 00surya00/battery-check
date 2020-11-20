# Simple Battery Alert

Sends a notification when battery is below and above the set limit.
(to reduce charging to 100% each time hence reducing the battery cycles in wear,
as to keep the charge between the set `$low` and `$high`)

### Prerequisites
 * `bash`
 * `upower` module
 * `x11`
 * `awk`
 * `notify-send`
 * `crontab`
 All of these are available by default on most of ubuntu based distros

### Installing

 * Edit the `battery-check` change the values of
      * `high` maximum limit while charging
      * `low` minimum limit while discharging
 * Copy the `battery-check` script to `<any-path-you-may-like>` make sure its executable
 * Add a crontab using `crontab -e`
 * Add the following `*/5 * * * * <any-path-you-may-like>` to the crontab and save

## Authors

* **Surya Hebbar** 

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* This is a simple script, just to get me started how i should make readme files and handle in the repo
