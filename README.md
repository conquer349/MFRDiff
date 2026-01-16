

## 1. Create Environment
- Create Conda Environment
```
conda create your_environment
conda activate your_environment
```
- Install Dependencies

We strongly recommend the configurations in the requirements.txt, for some old versions of dependencies may not support some new functions.

## 2. Prepare Your Dataset

you should list your dataset as the followed rule:
```bash
# Infrared and Visible image fusion:
    dataset/
        dataset1/
            train/
                 fused/
                 Infrared/
                 Visible/
            test/
                Infrared/
                Visible/
            val/
                Infrared/
                Visible/ 
        dataset2/           
```

## 4. Train
```shell
python train_redidual.py
```
Place the trained weights in the directory ./weight.

## 5. Testing
Modify path/resume_state to your weight path.
```shell
python infer_residual.py
```
