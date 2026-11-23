# Two ways to write a .gitignore

A `.gitignore` file tells git which files to leave out of version control. To use one of the examples here, copy it into your project root and rename it to `.gitignore`.

## Blacklist: `gitignore_blacklist`

Track everything, except what is listed.

```
pvt/
.Rhistory
.Rproj.user/
```

- Good default for most projects: new files are tracked automatically.
- Risk: anything you forget to list ends up in the repository, e.g. a large data file or a private note.

## Whitelist: `gitignore_whitelist`

Ignore everything, except what is listed with a leading `!`.

```
*
!.gitignore
!README.md
```

- Good when a folder holds mostly things that must not be shared, e.g. restricted data or private material: nothing is tracked unless you allow it explicitly.
- Risk: new files are silently left out until you add them to the list.
- `*` also ignores subfolders. To allow a folder and its contents, list the folder and its contents, e.g. `!code/` and `!code/**`.

## Which one to use

Use a blacklist for the project as a whole. Use a whitelist inside a folder whose contents should stay local by default, such as `data/` when the data cannot be shared: then only the files you allow, e.g. the data `README.md`, become public.
