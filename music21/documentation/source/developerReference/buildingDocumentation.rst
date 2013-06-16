.. _buildingDocumentation:


Building Documentation
==================================

Creating or updating the music21 documentation requires a few additional programs to be installed, 
most importantly one called Sphinx. Sphinx is a documentation generator that uses 
reStructuredText (rst) as its markup language and outputs HTML documents. 



**1) Installing setuptools**

software that makes it easy to download, build, upgrade, and uninstall Python packages. 
To download, go to http://pypi.python.org/pypi/setuptools and follow the instructions for whichever 
system you’re running. Be sure to get the version of setuptools that corresponds to the 
version of python you’re using as well (they’re all listed at http://pypi.python.org/pypi/setuptools#files). 
the egg version that you downloaded). For Python 2.7, it’ll look like this:
	
	
	
	
http://peak.telecommunity.com/DevCenter/EasyInstall?action=highlight&value=EasyInstall)




Once setuptools is installed, head to http://pypi.python.org/pypi/Sphinx/1.0.7 to download 
the Sphinx egg that corresponds to your version of Python.
the directory depending on where you saved the egg). 



Once that finishes running, go to Eclipse and under the ``buildDoc`` folder of ``trunk``, open ``build.py`` and run it. 
HTML documents should be generated and stored in ``music21/docs/html``, which you can then open in your web browser.
Static documentation goes in the ``buildDoc/staticDocs`` folder.  It is tested by running ``test/testDocumentation.py``.

To add a module to ``buildDoc``, it needs to be listed twice, first at the top import then in the list of modules below.
Keep all modules in alphabetical order.