Glade official git repository is hosted by the GNOME foundation at
git.gnome.org

Mailing List
~~~~~~~~~~~~
Glade discussion takes place on glade-devel@lists.ximian.com

To subscribe or to consult archives visit
	http://lists.ximian.com/mailman/listinfo/glade-devel


GitLab
~~~~~~~~
Glade bugs are tracked at

	https://gitlab.gnome.org/GNOME/glade


GIT
~~~
You can browse the source code at https://gitlab.gnome.org/GNOME/glade
To check out a copy of Glade you can use the following command:

	git clone https://gitlab.gnome.org/GNOME/glade.git

Patches
~~~~~~~
Patches must be in the unified format (diff -u) and must include a
ChangeLog entry. Please send all patches to bugzilla.

It is better to use git format-patch command

git format-patch HEAD^

Coding Style
~~~~~~~~~~~~
Code in Glade should follow the GNOME Programming Guidelines
(http://developer.gnome.org/doc/guides/programming-guidelines/),
basically this means being consistent with the sorrounding code.
The only exception is that we prefer having braces always on a new line
e.g.:

if (...)
  {
    ...
  }

Note however that a lot of the current codebase still uses the following
style:

if (...) {
  ...
}

Over time we'll migrate to the preferred form.

Naming conventions:
- function names should be lowercase and prefixed with the
  file name (or, if the function is static and the name too long,
  with an abbreviation), e.g:
  glade_project_window_my_function () 
  gpw_my_loooooooooong_named_fuction ()
- variable names should be lowercase and be short but self explanatory;
  if you need more than one word use an underscore, e.g:
  my_variable

Also try to order your functions so that prototypes are not needed.



