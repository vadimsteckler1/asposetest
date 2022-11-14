Usage
=====

.. _installation:

Retrieving supported file formats
---------------------------------

The following code sample demonstrates how to get supported file formats list::

   IEnumerable<FileType> supportedFileTypes = FileType
	.GetSupportedFileTypes()
	.OrderBy(f => f.Extension);

   foreach (FileType fileType in supportedFileTypes)
	Console.WriteLine(fileType);

