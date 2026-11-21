360° RENDERS FOR THE TOUR
=========================

Put the 3D artist's panoramas in this folder, then redeploy the site:
drag the whole site folder onto the Deploys page of the Netlify project.

One file per camera point (numbers and positions are in the artist brief):

  foyer.jpg      vestibule.jpg  gallery.jpg    living.jpg     ballv.jpg
  kitchen.jpg    dining.jpg     sitting.jpg    spa.jpg        br1.jpg
  br2.jpg        br3.jpg        powder.jpg     br1toilet.jpg  br2toilet.jpg
  br3toilet.jpg  westbal.jpg    bal1.jpg       bal2.jpg       coat.jpg
  br1dress.jpg   br2dress.jpg   br3dress.jpg   utility.jpg    store.jpg

Each file is an equirectangular JPEG, exactly twice as wide as it is tall
(8192 x 4096 recommended), with the centre of the image facing south, towards
the sea. The tour finds the files by name. Rooms without a file keep showing
the 3D preview.

manifest.json is optional. It turns renders that arrived facing the wrong way:
  { "yaw": { "living": 12.5 } }     degrees; a positive value turns the render right
The Align tool on the site (360° tour > Settings > Manage final renders) works
the value out and downloads a ready manifest.json.
