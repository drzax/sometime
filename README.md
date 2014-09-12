# Proposal

This repository is a proposal for the creation of `sometime.js` which is intended 
to be a library for parsing and representing inexact dates and times.

Comments and feedback most welcome.

## Vague requirements

Ideally this library would:

- Parse natural language dates to the fullest extent possible
- Represent inexact dates in a useful (hopefully standard) way
- Support parsing relative dates
- (Maybe) support intervals
- Not have dependencies on monolithic date libraries like [moment.js](http://momentjs.com/)
- Stay focused on parsing, and avoid implementing a formatter
- Collections of parsed dates/times (including intervals and inexact dates) should be sortable

Some strings which should be parsable:

- Late 2008
- August 2009
- November 24, 2009
- November-December 2009
- 2010
- Three years ago

# Prior art

## Parsing libraries

There are a few libraries with similar aims:

- [date](https://github.com/MatthewMueller/date)
- [chrono](https://github.com/wanasit/chrono) 

The one issue all existing libraries seem to have is that they are incapable of
storing or representing in-exact dates. The Chrono library comes closeset to the 
mark in this respect.

## Representation of inexact dates

The closest thing to a standard for representing inexact dates and times seems
to be the [EDTF](http://www.loc.gov/standards/datetime/pre-submission.html) standard
proposed by Library of Congress.

# Notes

Potentially useful implementations: 
- [EDTF validator in JS](https://gist.github.com/ptgolden/2791172)
