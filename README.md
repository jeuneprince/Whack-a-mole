# Whack-a-mole
CRUD IN HIGHSCORES
Dans la page "HIGHSCORES", se trouve un liste de scores qui peuvent etre modifiés en swipant la donnée de la droite vers la gauche ou supprimés en swipant la donnée de la gauche vers la droite. Le code de cette page est visible dans la class HighScoresViewState.
Pour la modification, je n'ai pas crée de page ni de textcontroller pour en remettre donc je l'ai codée en dur directement dans le code a la ligne 958 (await HighscoresDB.instance.update(Highscores(id:snapshot.data![index].id! ,date: "19-10-2022", name: "Souleymane", score: "99"));)
Ensuite pour l'ajout, un bouton vous amene sur une nouvelle page dans laquelle vous pourrez ajouter la date, le nom et le score vu que l'id est généré automatiquement dans la bd. Il n'y a qu'une seule validation pour le "required".
