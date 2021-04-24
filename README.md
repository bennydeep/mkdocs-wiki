# Onboarding

## Hogyan használd

Ha szerkeszteni akarod, kell majd jogsi neked a firebasehez.

Kezdd azzal hogy fork-olod a repository-t, aztán azt klónozd le.

ami mindenképp kelleni fog
```bash
npm install firebase-tools -g
pip install mkdocs
pip install mkdocs-material
```
ugye masterre meg van csinálva a ci-cd és ott automatikusan lebuildeli és ki is deployolja a weboldalt  
a firebase cli-t be kell magadnak configolni, saját accra, amit kapsz tokent berakni stbstb
```bash
mkdocs build
firebase deploy --token $FIREBASE_TOKEN --only hosting 
#firebase deploy --project syscops-onboarding
```
a második féle firebase deploy csak akkor működik ha már van service accountod, és a secret json is be van neki adva  
ha minden adott akkor már szerkesztheted is az onboarding oldalunkat.  
ha majd lesz jogsi hogy masterre pusholj, ott ugye megcsinálja magától.




