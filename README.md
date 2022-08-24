# multerupload

To use multer first install multer 

Add this folder to your project in backed to use.

After this in your routes import this code

const { upload } = require('../middlewares/fileupload')

and then use it like 

// ******************** //

router.post('/single', upload.single("image"), (req, res) => {
     console.log(req.file);
  res.send("Single FIle upload success");
})
