# software-carpentry-workshops
Document process for setting up a [Software Carpentry workshop](http://software-carpentry.org/workshops) at [NIST](http://www.nist.gov)

1. Book a room at http://nistrooms.nist.gov

  Things to consider:

  - conference rooms near the Gaithersburg cafeteria are better for keeping breaks from 
    dragging on too long

  - least confusing if the workshop is in the same room for both days

  - novice/advanced tracks mean two rooms for two full days. Book early!

2. Line up instructors (may need to iterate with 1.)

   - novice/advanced tracks mean three or four instructors *minimum*

3. Set up the workshop repository based on https://github.com/swcarpentry/workshop-template

   The following deviations from the template instructions *must* be made:

   - When importing the [workshop-template](https://github.com/swcarpentry/workshop-template) 
     repository, set the owner to `usnistgov` if possible. If you are
     unable to choose the `usnistgov` organization, then set the owner to
     your personal account on github and contact data@nist.gov to move the
     repository into the `usnistgov` organization. Choose a name for the
     repository of the form `YYYY-MM-DD-nist`.

   - Per NIST policy, you *must do your work in your repository's 
     `nist-pages` branch*. After you import the repository, 
     clone a local working copy and execute the following commands to 
     rename the primary branch:
     {{{
     git branch --move gh-pages nist-pages
     git push origin :gh-pages nist-pages
     }}}
     Push the content to the https://pages.nist.gov server by following 
     the instructions at http://inet.nist.gov/odi/github#github-pages.

     Note: templates are forthcoming and may conflict with the Software
     Carpentry templates.


