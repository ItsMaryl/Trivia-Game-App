# Trivia-Game-App
Java Trivia Quiz Application using Open Trivia Database API

## Περιγραφή
Χρησιμοποιώντας τη βιβλιοθήκη Trivia API που φτιάχνουμε στο αρχείο TriviaAPI (Μέρος Α) το project υλοποιεί ένα παιχνίδι γνώσεων (trivia quiz) σε Java.
Οι χρήστες μπορούν να απαντούν σε ερωτήσεις πολλαπλής επιλογής ή σωστό/λάθος και να διαγωνίζονται για υψηλότερο σκορ.

**Χαρακτηριστικά:**
-Κλήση API για την ανάκτηση ερωτήσεων που ικανοποιούν συγκεκριμένα κριτήρια.
-Λήψη των ερωτήσεων σε μορφή JSON (JSON response).
-Αποσειριοποίηση (deserialization) του response στα σχετικά Java Objects. Για το σκοπό αυτό, θα πρέπει να υλοποιήθηκαν και οι αντίστοιχες POJO  κλάσεις
- Επιλογή αριθμού ερωτήσεων, κατηγορίας, δυσκολίας και τύπου (multiple/boolean).
- Υπολογισμός σκορ: +10 για σωστή απάντηση, -5 για λάθος.
- Μέγιστο σκορ ανά συνεδρία.
- Φιλικό περιβάλλον με μηνύματα για κάθε ενέργεια του χρήστη.
- Ασφαλής διαχείριση εξαιρέσεων (exception handling) για αποτυχία ανάκτησης ερωτήσεων.
- Unit tests για κλάσεις όπως `HighScoreStore` και `GameConfig`.

---

## Απαιτήσεις
- Java 17+
- Maven
- Διαδίκτυο για πρόσβαση στο Open Trivia Database API
- JavaFX 20

---

## Εκτέλεση
Με Maven:
mvn clean javafx:run
ή άνοιγμα του project σε Eclipse/IntelliJ IDEA και εκτέλεση της κλάσης app.App

---

## Unit Tests

Υλοποιήθηκαν με JUnit για:
-Έλεγχο TriviaService (ερωτήσεις από βιβλιοθήκη).
-Έλεγχο HighScoreStore (update/reset).
-Έλεγχο GameConfig και παραμέτρων παιχνιδιού.

Για εκτέλεση:

mvn test
