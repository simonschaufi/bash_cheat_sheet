# Bash Cheat Sheet

## Replace tabs with spaces in xml files

```bash
find ./typo3/sysext/ -type f -name "*.xml" \
-exec sed -i 's/\t/    /g' {} \;

find ./Build -name "*.xml" -not -path "./Build/node_modules/*" \
-exec sed -i 's/\t/    /g' {} \;
```
