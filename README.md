# Compact-Simplex-Algorithm-in-APL
Update and correction to 1985 simplex algorithm published in APL Quote Quad.  This algorithm solves linear programs within Dyalog APL, providing both primal and dual solutions as well as alternative primal solutions if they exist.

In 1985 I published Compact Simplex Method under Algorithms in APL Quote Quad.  At the time, my intention was to display minimalist code which could provide straightforward solution to modest linear programs within APL itself.  Today, of course, we have very fast PCs with gobs of memory and efficient, open-source LP solvers in R and Python, including Py’n’APL, an APL-Python interface to access such solvers within APL.

Ordinarily, I would not revisit an old algorithm that I hadn’t accessed in decades.  However, I have received an extensive stream of alerts from academia.edu which indicates that researchers are viewing my old published algorithm.  This motivated me to review my algorithm to make sure it would still work on the modern Dyalog APL platform and that it was producing accurate results.  In that context, I found that it needed some cleanup in terms of getting rid of underlined characters and superfluous rounding.  Most importantly, I found that signs in the optimal dual solution had to be corrected.  My revised code runs reasonably efficiently on Dyalog, even for a fairly large problem with randomized inputs.  This repository contains that revised simplex code plus examples.

The following files can be viewed in Dyalog or in Windows Notepad:
SIMPLEX is the basic optimization code.  INFEASIBLE, UNBOUNDED, PRODUCTION, TRANSPORATION, and LARGE are codes for examples using SIMPLEX.  SIMPLEX_EXAMPLE_EXECUTION contains example runs on Dyalog.

APL_QUOTE_QUAD is a PDF of my original 1985 article, including corrections, for easy reference.

Bob Agnew, raagnew1@gmail.com, raagnew.com

