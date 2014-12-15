git-hotfix(1) -- Create hotfix branch
===============================

## SYNOPSIS

`git-hotfix` [&lt;name&gt;]
`git-hotfix` [finish|fin|end|complete] &lt;name&gt;
`git-hotfix` [delete|del|remove|rm|clear] &lt;name&gt;

## DESCRIPTION

  Manage hotfix branch creation, deletion or merging back into integration branch. By default the master branch is considered the integration branch. 

  If the hotfix branch name is not given, then a list of hotfix branches will be displayed. 

## OPTIONS

  &lt;finish, fin, end, complete&gt;

  Merge and delete the hotfix branch.

  &lt;delete, del, remove, rm, clear&gt;

  Delete the hotfix branch from local and remote repositories.

  &lt;name&gt;

  The name of the hotfix branch.

## EXAMPLES

    $ git hotfix hotfix-123456
    ...
    $ git commit -m "Some changes"
    ...
    $ git checkout master
    $ git hotfix finish hotfix-123456

## AUTHOR

Written by Gerard Hickey &lt;<hickey@kinetic-compute.com>&gt;

## REPORTING BUGS

&lt;<https://github.com/hickey/git-extras/issues>&gt;

## SEE ALSO

&lt;<https://github.com/hickey/git-extras>&gt;
