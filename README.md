The ultimate objective of our project is to identify and replace individuals within an image with the background seamlessly.
We have divided the task into two distinct objectives:

  Objective 1: Detect People and Return their Masks 
    The first objective is to train deep learning models to accurately detect individuals in images
    and generate corresponding masks delineating their outlines, crucial for the mission's
    success in seamlessly replacing people with background elements.

    Model Training and Evaluation:
      In our pursuit of the best model, we trained five models and searched for the best
      Intersection over Union (IOU). Each model performed predictions on the test data, and the
      results were analyzed. To optimize efficiency and ensure that our progress was not lost, we
      saved the weights of all trained models to a file, which was automatically transferred to backup.
      This precautionary measure ensured that in the event of a session timeout or data
      clearance, we retained the valuable model weights.
      Based on the results, the Unet (pix2pix) model demonstrated the highest accuracy
      (0.9406) and mean IOU (0.8168) while showing the lowest loss (0.1480), thus being selected
      as the optimal model for the first objective.
    
  Objective 2: Replace Masks with Background
    The second objective involves taking the generated masks and corresponding images, and
    seamlessly replacing the masked regions with background elements.


  
  
