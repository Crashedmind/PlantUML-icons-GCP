# Generating the PlantUML Icons for GCP
The tool used to generate this icon set is based on https://github.com/awslabs/aws-icons-for-plantuml (where modification of the script is permitted per the license).
The script is made generic to be able to process other icon sets.

See symbols.md for a list of all the icons with associated image.


cd scripts/

python3 icon-builder.py --check-env 

python3 icon-builder.py --create-config-template

cp config-template.yml config.yml 
Manually change the default color to Google Blue 
GCPBlue: "#4285f4" color from svgs but looks anemic in rendered puml - so use GCPBlue: "#036ffc" instead

python3 icon-builder.py 