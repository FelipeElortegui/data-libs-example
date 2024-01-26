# Ejemplo para crear repo big-data-libs con submodulos

git submodule add git@github.com:FelipeElortegui/dsl-submodule-example.git libs/delivery/dsl
git submodule init
git submodule update

git add .
git commit -m "Add dsl Submodule"
git push

# Ejemplo para actualizar submodulo desde otro repo

cd libs/delivery/dsl
git fetch
git merge origin/main
cd ../../../
git add libs/delivery/dsl
git commit -m "Updated submodule"
git push