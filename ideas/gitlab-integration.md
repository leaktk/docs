# GitLab Integration

Make it compatible as a custom GitLab scanner

https://www.youtube.com/watch?v=timMbl5SP-w

## Notes

It may make sense to create a separate thing that takes the scanner output and
maps it to keep the core scanner agnostic. This could be either by importing
the scanner as a library or piping the output of one to another.

If there aren't any issues with piping the output of one to another, I would
prefer that method.
