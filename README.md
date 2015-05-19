# forward2reverse
 
**forward2reverse** is a Ruby script for converting A and AAAA (forward DNS) records to PTR (reverse DNS) records. It can read zone files as input, and will ignore lines which don't contain A or AAAA DNS records.

## Example Usage

1. Convert a single A record:

        echo "example.com. A 1.2.3.4" | forward2reverse

2. Convert a list of A and/or AAAA records listed in a file. Other record types will be ignored:

        cat zone-file | forward2reverse

## Installation

1. Verify that you have [Ruby](https://www.ruby-lang.org/) 1.9.3 (released October 2011) or later installed:

        ruby --version

    Earlier versions may also work, but are untested.

2. Download and extract the tarball:

        wget https://github.com/mrideout/forward2reverse/archive/v0.1.tar.gz
        tar -xzf v0.1.tar.gz
        cd forward2reverse-0.1

3. Make **forward2reverse** executable:

        chmod 755 forward2reverse

4. Optionally, move **forward2reverse** into a directory that's in your PATH. For example:

        sudo mv forward2reverse /usr/local/bin/
 
## Contributing
 
1. Fork it!

2. Create your feature branch:

        git checkout -b my-new-feature

3. Commit your changes:

        git commit -a -m 'Add some feature'

4. Push to the branch:

        git push origin my-new-feature

5. Submit a pull request.
 
## History

[Matt Rideout](https://www.mattrideout.com/) wrote and released **forward2reverse** in May 2015. 
 
## License
 
**forward2reverse** is open source software released under the [MIT License](http://www.opensource.org/licenses/MIT).

