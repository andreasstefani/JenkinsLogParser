# JenkinsLogParser
Each line in the file specifies a level (ok/error/warning/info/start) and a regular expression (based on java.util.regex.Pattern) delimited by slashes ("/") to look for in order to mark the line as matching that level.

## ok/error/warning
Used to identify problem lines.

## info
These lines are highlighted blue in the report. They are used to create a set of links into the report for quick access to certain sections.

## start
Like info lines, they are highlighted blue in the report, and appear in the set of quick access links to the report. In addition, they are used for grouping the list of errors and warnings found in that section.

# Example
error /ERROR/
error /File not found/
error /The following build commands failed/

warning /[Ww]arning/
warning /WARNING/

ok /Warning: no symbols in executable/
