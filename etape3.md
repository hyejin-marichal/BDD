#Etape3

A l’aide de PhpMyAdmin, remplir cette base avec des données de tests significatives en
respectant les conditions suivantes :

○ Une catégorie “loisirs” devra exister

 -
 INSERT INTO `category`(`Nom`) VALUES ('Loisir') 

○ Vous devez avoir à minima 5 auteurs, pour 2 d’entre eux, le pseudo sera “Matéo”
et “Valentine”

-
INSERT INTO `auteur`(`Pseudo`, `Nom`, `Prenom`) 
VALUES ('Matéo','Mama','Mimi'), ('Valentine','Vava','Vivi'), ('kiwi','Kaka', 'Kiki'), ('Sara','Sasa','Sisi'), ('Nemo','Nana','Nini')


○ Des articles devront avoir “Sport” dans leur titre et “Biathlon” dans leur texte

-
INSERT INTO `article`(`Titre`, `Texte`, `Date`, `importance`, `FinDate`, `Auteur_Pseudo`) 
VALUES ('Sport','Biathlon','2020-01-23','0','2020-01-29','Matéo')

○ Des articles devront être publiables aujourd’hui

- 
INSERT INTO `article`(
    `Titre`,
    `Texte`,
    `Date`,
    `importance`,
    `FinDate`,
    `Auteur_Pseudo`
)
VALUES(
    'Sport d''hiver',
    'wawawa Biathlon',
    '2020-01-20',
    '1',
    '2020-01-27',
    'Valentine'
),
(
    'Sport d''été',
    'kakakaka Biathlon',
    '2020-01-22',
    '1',
    '2020-01-28',
    'kiwi'
),
(   'Solde',
    'kakakaka soldesolde',
    '2020-01-22',
    '1',
    '2020-01-28',
    'Matéo'
),
(
    'Voyage',
    'newyork',
    '2020-01-19',
    '1',
    '2020-01-25',
    'Nemo'
),
(
    'Santé',
    'bien etre',
    '2020-01-20',
    '5',
    '2020-01-27',
    'Matéo'
),
(
    'Dance',
    'Dancence',
    '2020-01-23',
    '2',
    '2020-01-30',
    'Matéo'
)

○ Des commentaires contiendront “Bravo”, d’autres ne seront que “Sans avis”

- 
INSERT INTO `commnetaire`(
    `Text`,
    `Date`,
    `Auteur_Pseudo`,
    `Article_Titre`
)
VALUES(
    'Bravo',
    '2020-01-23 01:16:35',
    'kiwi',
    'Dance'
),(
    'Bravo',
    '2020-01-24 05:34:52',
    'Matéo',
    'Sport d\'été'
),(
    'Bravo',
    '2020-01-25 07:35:20',
    'Nemo',
    'Solde'
),(
    'Sans avis',
    '2020-01-26 10:16:00',
    'Valentine',
    'Sport'
),(
    'Sans avis',
    '2020-01-27 18:14:10',
    'Sara',
    'Sport d\'hiver'
),(
    'Sans avis',
    '2020-01-25 13:33:17',
    'Matéo',
    'Sport d\'hiver'
),(
    'Sans avis',
    '2020-01-24 08:23:00',
    'Sara',
    'Sport d\'hiver'
),(
    'Bravo',
    '2020-01-25 15:00:19',
    'Valentine',
    'Solde'
);


○ L’auteur “Matéo” devra commenter des articles qu’il a rédigé

-
INSERT INTO `commnetaire`(
    `Text`,
    `Date`,
    `Auteur_Pseudo`,
    `Article_Titre`
)
VALUES(
    'blablal',
    '2020-01-24 07:00:00',
    'Matéo',
    'Santé'
),(
    'wowowow',
    '2020-01-24 10:22:00',
    'Matéo',
    'Sport'
),(
    'kkkkkkk',
    '2020-01-25 00:12:42',
    'Matéo',
    'Dance'
),(
    'ddddddeeedede',
    '2020-01-26 11:00:53',
    'Matéo',
    'Solde'
);

