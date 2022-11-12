Feature-Rich PDF Annotator for C#/.NET Developers
===================================

**GroupDocs PDF Annotator** is a feature-rich tool for adding special notes and markups to PDFs. Its lightweight API architecture is artfully tailored to enable you to effortlessly incorporate it into your application.

With our Annotator your application will acquire the ability to add text annotations, highlights, callouts and other elements directly to the PDF without altering the original content. The annotations are saved to the document and can be viewed by using any PDF viewer. The annotated document can be then printed or forwarded in its completed form.

.. note::

   All annotations and markups can still be edited when you re-open the document
   
#Walk-through of an example annotation

To give you a taste of what GroupDocs Annotator brings to the table, here is an example using the simplest way to run a spider.

```c#
using (Annotator annotator = new Annotator("input.pdf"))
{
	AreaAnnotation area = new AreaAnnotation
    {
     	BackgroundColor = 65535,
        Box = new Rectangle(100, 100, 100, 100),
        CreatedOn = DateTime.Now,
        Message = "This is area annotation",
        Opacity = 0.7,
        PageNumber = 0,
        PenColor = 65535,
        PenStyle = PenStyle.Dot,
        PenWidth = 3,
        Replies = new List<Reply>
        {
        	new Reply
            {
            	Comment = "First comment",
                RepliedOn = DateTime.Now
            },
            new Reply
            {
            	Comment = "Second comment",
                RepliedOn = DateTime.Now
            }
        }
    };
    annotator.Add(area);
    annotator.Save("result.pdf");
}
```

* Collaborate with your co-workers using highlighting, callouts, and text annotations.
* As a teacher, present your onscreen lectures with PDF Annotator making notes in real time. Save the presentation and email it to your students for a study guide, then remove the markups for the next class and start fresh.
* Instructions in computer and appliance manuals can be highlighted to help you find them again easily.

Use the Annotator on your Tablet PC or touch-screen laptop for collaboration on the road.

Make hand-written notes to your PDF documents and e-mail them right from the PDF Annotator.

For more information on how the PDF Annotator can make your business, academic, and home computing better, refer to 
Contents
--------

.. toctree::

   usage
   api
