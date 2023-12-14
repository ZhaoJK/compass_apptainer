# compass conatiner for metabolic analysis

apptainer image for compass

Reference:
python image from https://github.com/docker-library/python/tree/master/3.8 
compass from https://github.com/YosefLab/Compass

How to use:
1. Download cplex from IBM according to instruction in compass 
2. Define silent file "installer.properties"
3. Run singularity/apptainer build
4. Analyze test data by "singularity exec ./compass_py37.sif --data /usr/local/lib/python3.7/site-packages/compass/Resources/Test-Data/tsv_format/expression.tsv --species homo_sapiens --num-processes 10 --output-dir . --temp-dir ."
