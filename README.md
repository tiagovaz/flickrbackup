flickrbackup - backup your flickr photos
----------------------------------------

flickrbackup is a simple python script which allows you to save a local copy of
your flickr photo sets. Run it with -h to see the options.

dependencies
------------

python, python-pyexiv2

settings
--------

    $ mv local_settings.py.in local_settings.py

Edit local_settings.py with your Flickr API Key and Secret

simple usage
------------

    $ ./flickrbackup -o <outputdir>

full options
------------

    Usage: flickrbackup [OPTIONS] -o OUTPUT_DIR

    Backup your flickr photos.

    Options:
      --version             show program's version number and exit
      -h, --help            show this help message and exit
      -o OUTPUT_DIR, --output_dir=OUTPUT_DIR
                            set the local directory where you want to store your
                            pictures
      -S BACKUP_SET, --set=BACKUP_SET
                            Specific set to backup
      -e, --metadata-exif   store flickr metadata (title, description etc) as EXIF
                            tags in your local files [default: False]
      -x, --metadata-xml    store metadata as default flickr XML files [NOT
                            IMPLEMENTED]
      -u, --metadata-update
                            update flickr metadata to your local files. Use this
                            option with -x and/or -e [default: False]
      -g, --html-gallery    generate a local HTML gallery [NOT IMPLEMENTED]

