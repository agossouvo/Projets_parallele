# Projets_secondaires
Bonjour à tous !

J'apprends intensivement à coder et je m'intéresse à la science des données, dans le but d'être embauché comme analyste de données en 2022.
Ce dépôt est destiné à divers projets secondaires et à des bouts de code avec lesquels je me suis amusé pendant mon apprentissage du codage.

Liste des projets :

Énoncé du problème : Prédiction des défauts de paiement des prêts automobiles

Les institutions financières subissent des pertes importantes en raison des défauts de paiement des prêts automobiles. Cela a conduit à un resserrement de la souscription des prêts automobiles et à une augmentation des taux de rejet des prêts automobiles. Le besoin d'un meilleur modèle de notation du risque de crédit est également soulevé par ces institutions. Cela justifie une étude visant à estimer les déterminants du défaut de remboursement des prêts automobiles. Une institution financière vous a engagé pour prédire avec précision la probabilité que le preneur de crédit/l'emprunteur ne rembourse pas son prêt automobile à la date d'échéance du premier versement mensuel équivalent (EMI). Les informations suivantes concernant le prêt et le preneur sont fournies dans les jeux de données :

Informations sur le preneur de crédit (données démographiques telles que l'âge, le revenu, la preuve d'identité, etc.) Informations sur le prêt (détails du versement, montant, EMI, ratio prêt/valeur, etc.) Données et historique du bureau (score du bureau, nombre de comptes actifs, statut des autres prêts, historique de crédit, etc.) Cela permettra de s'assurer que les clients capables de rembourser ne sont pas rejetés et que les déterminants importants peuvent être identifiés, ce qui peut être utilisé pour minimiser les taux de défaut.
Description des données contient train.csv et train.csv contient les données de formation avec les détails sur le prêt comme décrit dans le data_dictionary contient une brève description sur chaque variable fournie dans la formation et test.csv contient les détails de tous les clients et les prêts pour lesquels les participants doivent soumettre la probabilité de défaut.

submission.csv contient le format de soumission des prédictions par rapport à l'ensemble de test. Un seul csv doit être soumis comme solution.
Métrique d'évaluation Les soumissions sont évaluées sur l'aire sous la courbe ROC entre la probabilité prédite et la cible observée.


## DICTIONNAIRE DE DONNÉES : 

Variable : Nom Description<br>

UniqueID : Identifiant pour les clients <br>
loan_default : Défaut de paiement du premier EMI à la date d'échéance <br>
disbursed_amount : Montant du prêt déboursé <br>
asset_cost : Coût de l'actif <br>
ltv Loan to Value of the asset : (La loan to value ou LTV est un indicateur utilisé lors de l’octroi du prêt immobilier. Il consiste à faire un ratio entre le montant du crédit et la valeur d’achat du logement (hors droits de mutation et/ou d’acquisition). Plus ce ratio est élevé, plus le risque de l'emprunt est important.
La LTV est un ratio d'endettement. Il se calcule en rapportant le montant d'un emprunt à la valeur du bien acquis grâce à cet emprunt et/ou de l'actif donné en garantie de l'emprunt.
Il mesure ainsi, au moment n, le niveau d’endettement d’un emprunteur au regard de la valeur vénale de ses actifs immobiliers. Plus ce ratio est élevé, plus le risque de l'emprunt est important.<br>
branch_id : Succursale où le prêt a été déboursé <br>
supplier_id : Concessionnaire du véhicule où le prêt a été déboursé<br>
manufacturer_id : Fabricant du véhicule (Hero, Honda, TVS, etc.) <br>
Current_pincode : Code postal actuel du client Date.de.naissance Date de naissance du client <br>
Employment.Type : Type d'emploi du client (salarié/indépendant) <br>
DisbursalDate : Date du déboursement <br>
State_ID : État du déboursement <br>
Employee_code_ID : Employé de l'organisation qui a enregistré le déboursement. <br>
MobileNo_Avl_Flag : si le numéro de mobile a été partagé par le client, le drapeau est 1.<br> 
Aadhar_flag  : si l'aadhar a été partagé par le client alors marqué comme 1 <br>
PAN_flag : si le pan a été partagé par le client puis marqué comme 1 <br>
VoterID_flag : si l'électeur a été partagé par le client puis marqué comme 1 <br>
Driving_flag : si le client a partagé son permis de conduire, le drapeau indique 1. <br>
Passport_flag : si le passeport a été partagé par le client, puis marqué comme 1.<br> 
PERFORM_CNS.SCORE : Score du bureau <br>
PERFORM_CNS.SCORE.DESCRIPTION : Description du score du bureau <br>
PRI.NO.OF.ACCTS : nombre total de prêts contractés par le client au moment du décaissement Les comptes primaires sont ceux que le client a contractés pour son usage personnel<br>
PRI.ACTIVE.ACCTS : nombre de prêts actifs contractés par le client au moment du décaissement PRI.OVERDUE.ACCTS nombre de comptes en défaut au moment du décaissement <br>
PRI.CURRENT.BALANCE : total du capital restant dû des prêts actifs au moment du déboursement. <br>
PRI.SANCTIONED.AMOUNT : Montant total qui a été sanctionné pour tous les prêts au moment du décaissement. <br>
PRI.DISBURSED.AMOUNT : montant total qui a été décaissé pour tous les prêts au moment du décaissement. <br>
