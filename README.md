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
