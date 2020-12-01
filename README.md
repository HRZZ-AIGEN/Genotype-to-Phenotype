# Genotype-to-Phenotype
 
 A) **Mapiranje_fenotipova-Report.pdf** - U svhu validacije ProTraits predvidjenih fenotipova za bakteriske sojeve, prikupljeni su podaci s BacDive baze podataka (engl. Bacterial Diversity Metadatabase) koja sadrzi informacije o taksonomiji, morfologiji, fiziologiji te nacinu izolacije i kultivacije preko 64 000 bakterijskih sojeva. U danom izvjescu ukratko je prikazan pristup skidanja podataka s BacDive baze i mapiranje fenotipova sojeva na fenotipove sojeva predvidjenih od strane ProTraitsa. 
 
 B) **KOVER** pristup obuhvaca implementaciju SCM (engl. Set Covering Machines) i CART (engl. Classification and regression trees) metoda zasnovanim na pravilima u svrhu otkrivanja genomskih biomarkera. KOVER mogucava racunalno ucinkovito treniranje modela bez potrebe za ucitavanjem cjelih skupova podataka u memoriju racunala te daje intepretabilne modele bazirane na k-merima. 

 Skup pravila kod oba implemetirana modela rezultiraju logickim vrijednostima, True ili False, ovisno o prisutnosti ili odsutnosti odredjenog k-mera u sekvenci genoma. Logicke kombinacije pravila mogu biti konjunkcije (logical-AND) cime se pozitivan razred dodjeljuje ako sva pravila odgovaraju izlazu True, ili disjunkcije (logical-OR) cime se dodjeljuje pozitivan razred ako barem jedno pravilo odgovara izlazu True. Za razliku od SCM pristupa, CART omogucava klasifikaciju s proizvoljnim brojem razreda. 

 Podaci su prikupljeni s PATRIC baze podataka (https://docs.patricbrc.org/user_guides/ftp.html). Nakon pretprocesiranja, ukljucuju 107 binarnih skupova s barem 25 bakterijskih izolata za svaki fenotip (12 humanih patogena i 56 antibiotika). Podaci su podjeljeni na dva razreda s obzirom na podloznost ili rezistentnost na odredjeni antibiotik (engl. susceptible/resistant). Za svaku od bakterijskih vrsta genomske sekvence su podjeljenje na preklapajuce k-mere (k=31) kojima je dodjeljena logicka vrijednost s obzirom na prisutnost ili odsutnost odgovarajuceg k-mera u genomskoj sekvenci. 

 **Report.pdf** - A short summary of pappers by Drouin et al. regarding Kover workflow. 

 Kover je napisan u Pythonu i Cythonu. Na danom linku (https://aldro61.github.io/kover/index.html) nalazi se tutorial za instalaciju i koistenje Kovera.

 [1] Drouin, A., Giguère, S., Déraspe, M., Marchand, M., Tyers, M., Loo, V. G., Bourgault, A. M.,Laviolette, F. & Corbeil, J. (2016). Predictive computational phenotyping and biomarker discovery using reference-free genome comparisons. BMC Genomics, 17(1), 754.
 [2] Drouin, A., Letarte, G., Raymond, F., Marchand, M., Corbeil, J., & Laviolette, F. (2019)Interpretable genotype-to-phenotype classifiers with performance guarantees. Scientific Reports, 9(1), 4071.
