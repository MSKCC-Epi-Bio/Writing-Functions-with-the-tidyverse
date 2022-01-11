# Writing-Function-with-the-tidyverse

Tweet-sourced resources
1. https://www.vishalkatti.com/posts/2021-07-17-programmingwithdplyr/
2. https://ayushbipinpatel.github.io/R-for-Data-Analysis/functions-and-functional-programming.html#1
3. https://dplyr.tidyverse.org/articles/programming.html
4. https://www.brodrigues.co/blog/2019-06-20-tidy_eval_saga/
5. https://speakerdeck.com/chendaniely/learning-tidy-evaluation-by-reimplementing-dplyr
6. https://speakerdeck.com/jennybc/tidy-eval-in-context?slide=1
7. https://rlang.r-lib.org/
8. https://laderast.github.io/posts/2017-12-19-understanding-tidyeval/


**Tidy Evaluation at Open Study Group**

Section 1: Build a function that uses tidyverse unquoted args internally (LAVERY)
  - Passing strings to dplyr verbs
  - `across()` and `any_of()` and `all_of()`
  - .data[[varname]] (also introduce .env pronoun)
  - `rlang::sym()`  and `rlang::syms()`, e.g. select(!!rlang::sym(varname))

  Let’s build a function that creates a ggplot….maybe a survival curve?

Section 2: Build a function that uses unquoted args itself (SJOBERG)
  - {{ }}
  - First, easy option is to just immediately convert unquoted variable names to strings
  - varname <- dplyr::select(data, {{ varname }}) |> names()
  - enquo() and bang-bang (!!)

  Recreate `dplyr::select()`

40 minutes of instruction
20 minutes of practice (stay on the line if you’re interested)
Instruction will focus on section 1 skills

Xaringan slides will live in epi/bio gh org
