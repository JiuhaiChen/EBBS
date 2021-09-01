To run the code on your dataset, it's necessary to prepare the files in the right format.

There should be at least X.csv (node features), y.csv (target labels), graph.graphml (graph in graphml format).

You can also have cat_features.txt specifying names of categorical columns.

You can also have masks.json specifying train/val/test splits.

Then run the command:

python run.py   --datasets  your_datasets   --task regression   --X_lam 20.0 --X_step 5  --y_lam 2.0 --y_step 5  --lr 0.1    --label_smooth  --error_smooth


(Very simple example on our dataset House: zip the datasets and then run python run.py   --datasets  house   --task regression   --X_lam 20.0 --X_step 5  --y_lam 2.0 --y_step 5  --lr 0.1    --label_smooth  --error_smooth)
