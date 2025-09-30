# daily_checkin_app
Application Flutter de vérification quotidienne avec SMS automatique
# ✅ Daily Check-In App

Application Flutter de **vérification quotidienne**.  
Elle permet à l'utilisateur de confirmer qu'il va bien chaque jour.  
Sinon, l'app **envoie un SMS automatiquement** à un contact d'urgence même si elle est fermée.

---

## 🚀 Fonctionnalités

- ⏱️ Minuteur de 24h redémarré à chaque "check-in"
- 🔕 Notification locale 10 minutes avant la fin
- 📩 Envoi automatique d’un SMS d’alerte si l’utilisateur ne répond pas
- ⚙️ Paramétrage du numéro et du message
- 💤 Fonctionne en arrière-plan grâce à `workmanager`

---

## 📸 Aperçu

| Écran principal | Paramètres |
|-----------------|------------|
| ![home](https://via.placeholder.com/200x400?text=Check-In+UI) | ![settings](https://via.placeholder.com/200x400?text=Settings+UI) |

---

## 📱 Installation locale

### 1. Cloner le projet

```bash
git clone https://github.com/ton-utilisateur/daily_checkin_app.git
cd daily_checkin_app
<uses-permission android:name="android.permission.SEND_SMS"/>
<uses-permission android:name="android.permission.RECEIVE_SMS"/>
<uses-permission android:name="android.permission.READ_SMS"/>
<uses-permission android:name="android.permission.RECEIVE_BOOT_COMPLETED"/>
<receiver
    android:name="be.tramckrijte.workmanager.WorkManagerBroadcastReceiver"
    android:enabled="true"
    android:exported="true">
    <intent-filter>
        <action android:name="android.intent.action.BOOT_COMPLETED"/>
        <action android:name="android.intent.action.REBOOT"/>
    </intent-filter>
</receiver>
defaultConfig {
    ...
    minSdkVersion 21
}
// Pour test rapide : 
initialDelay: Duration(minutes: 2),

---

## ✅ Étapes suivantes

1. Crée un fichier `README.md` dans ton dépôt (ou modifie celui déjà créé).
2. Colle le contenu ci-dessus.
3. Commit & push :

```bash
git add README.md
git commit -m "Ajout du README complet"
git push
