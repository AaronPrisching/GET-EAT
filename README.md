[README.md](https://github.com/user-attachments/files/22386051/README.md)
# GetEat - Team-Lunch-Management System

Ein professionelles Team-Lunch-Management-System mit Voting, Bestellungen und intelligenter Koordination für Unternehmen.

## 📋 Inhaltsverzeichnis

- [Überblick](#überblick)
- [Features](#features)
- [Installation](#installation)
- [Verwendung](#verwendung)
- [Admin Dashboard](#admin-dashboard)
- [Benutzerrollen](#benutzerrollen)
- [Technische Details](#technische-details)
- [Konfiguration](#konfiguration)
- [Mobile Optimierung](#mobile-optimierung)
- [Support](#support)

## 🎯 Überblick

GetEat ist eine Single-Page-Application (SPA) für das Management von Team-Lunches. Das System ermöglicht es Teams, demokratisch über Restaurants abzustimmen, Bestellungen zu koordinieren und PayPal-Zahlungen zu verwalten.

### Hauptfunktionen:
- **Demokratisches Voting** für Restaurant-Auswahl
- **Integrierte Bestellverwaltung** mit Warenkorb
- **PayPal-Integration** mit QR-Code-Zahlungen
- **Admin Dashboard** für vollständige Systemkontrolle
- **Mobile-optimiert** für alle Geräte
- **Automatische Datenpersis­tierung** im Browser

## ✨ Features

### 🗳️ Voting System
- **Wochentags-basiertes Voting** (Montag bis Freitag)
- **Restaurant-Auswahl** pro Tag konfigurierbar
- **Demokratische Abstimmung** mit Mehrheitsentscheidung
- **Live-Updates** der Voting-Ergebnisse
- **Teilnehmer-Management** für jeden Tag

### 🛒 Bestellsystem
- **Intelligenter Warenkorb** mit Mengensteuerung
- **Restaurant-spezifische Menüs** mit Preisen
- **Automatische Kostenberechnung**
- **Bestellhistorie** für alle Nutzer
- **Order-Management** mit Status-Tracking

### 💳 PayPal Integration
- **QR-Code-Generierung** für Zahlungen
- **Automatische PayPal-Modals** nach Bestellung
- **Zahlungsstatus-Tracking** (Bezahlt/Ausstehend)
- **Admin-Upload** für PayPal-Codes
- **Zahlungsbestätigung** durch Admin

### 👥 Benutzerverwaltung
- **Registrierte Benutzer** mit vollständigen Profilen
- **Aktive Benutzer** aus Voting/Bestellaktivitäten
- **Benutzer-CRUD-Operationen** (Erstellen, Bearbeiten, Löschen)
- **Passwort-Reset** mit Standard-Passwort (12345678)
- **Benutzerstatistiken** (Ausgaben, Bestellanzahl)

### 🏪 Restaurant-Management
- **Restaurant-CRUD** (Hinzufügen, Bearbeiten, Löschen)
- **Menü-Management** pro Restaurant
- **Gerichte bearbeiten** (Name, Preis)
- **Kategorie-Verwaltung**
- **Tägliche Restaurant-Auswahl** für Voting

## 🚀 Installation

### Voraussetzungen
- Moderner Webbrowser (Chrome, Firefox, Safari, Edge)
- Webserver (optional, kann auch lokal geöffnet werden)

### Setup
1. **Repository klonen oder Datei herunterladen**
   ```bash
   # Datei herunterladen
   wget [repository-url]/index.html
   ```

2. **Direkt im Browser öffnen**
   ```bash
   # Lokaler Pfad
   file:///pfad/zur/datei/index.html
   
   # Oder über Webserver
   http://localhost/geteat/index.html
   ```

3. **Fertig!** - Keine weitere Konfiguration erforderlich

## 💻 Verwendung

### Für normale Benutzer

#### 1. **Voting**
- Navigiere zu "Voting" im Menü
- Wähle einen Wochentag aus
- Stimme für dein bevorzugtes Restaurant ab
- Melde dich für die Teilnahme an

#### 2. **Bestellen**
- Klicke auf "Menü anzeigen" nach dem Voting
- Wähle Gerichte aus und füge sie zum Warenkorb hinzu
- Überprüfe deine Bestellung und klicke "Bestellen"
- Scanne den PayPal QR-Code für die Zahlung

#### 3. **Profil verwalten**
- Öffne das Profil über das Menü
- Zeige deine Bestellhistorie an
- Aktiviere Benachrichtigungen (optional)

### Für Administratoren

#### Admin-Zugang
- **Standard-Login**: `admin` / `admin123`
- Oder über die erlaubten Admin-Benutzer

## 🛠️ Admin Dashboard

Das Admin Dashboard bietet vollständige Kontrolle über das System:

### 📊 Übersicht
- **Benutzerstatistiken** (Aktive Benutzer, Bestellungen)
- **Umsatzübersicht** mit Gesamtsummen
- **System-Metriken** (Restaurants, Bestellungen)
- **CSV-Export** für Buchhaltung
- **Push-Benachrichtigungen** senden

### 🚗 Abholung & PayPal Management
- **Bestellungen freischalten/sperren** pro Tag oder alle
- **Abholer-Verwaltung** pro Wochentag
- **PayPal-Code Upload** mit Bildvorschau
- **Voting-Management** (Stimmen löschen)
- **Bestellstatistiken** pro Tag

#### Zentrale Bestellungssteuerung
```javascript
// Alle Tage freischalten
🔓 Alle freischalten

// Alle Tage sperren  
🔒 Alle sperren
```

### 🏪 Restaurant Management
- **Restaurants hinzufügen/bearbeiten/löschen**
- **Menü-Artikel verwalten** (Name, Preis)
- **Kategorien zuweisen**
- **Tägliche Restaurant-Auswahl** konfigurieren

### 👥 Benutzer Management
- **Benutzer erstellen** mit Name und E-Mail
- **Benutzer bearbeiten** (Name, E-Mail ändern)
- **Passwort zurücksetzen** auf Standard (12345678)
- **Benutzer löschen** mit kompletter Datenbereinigung
- **Aktive zu registrierten Benutzern** konvertieren

### 📦 Bestellungen Management
- **Alle Bestellungen anzeigen** chronologisch sortiert
- **Datumsfilter** für spezifische Tage
- **Zahlungsstatus** verwalten (Bezahlt/Ausstehend)
- **Bestellungen löschen** mit Bestätigung
- **Bestellungsdetails** mit Artikeln und Preisen

### ⚙️ System-Einstellungen
- **Admin-Passwort ändern**
- **Erlaubte Admin-Benutzer** verwalten
- **System-Konfiguration**

## 👤 Benutzerrollen

### **Normale Benutzer**
- Voting-Teilnahme
- Bestellungen aufgeben
- Profil verwalten
- Bestellhistorie einsehen

### **Administratoren**
- Vollzugriff auf alle Funktionen
- Restaurant-Management
- Benutzer-Verwaltung
- System-Konfiguration
- Bestellungs-Koordination

## 🔧 Technische Details

### Architektur
- **Single-Page-Application** (SPA)
- **Vanilla JavaScript** (ES6+)
- **CSS3** mit Custom Properties
- **LocalStorage** für Datenpersistierung
- **Responsive Design** (Mobile-First)

### Browser-Unterstützung
- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

### Datenspeicherung
```javascript
// Lokale Speicherung im Browser
localStorage.setItem('geteat-state', JSON.stringify(state));

// Automatische Wiederherstellung beim Laden
const savedState = JSON.parse(localStorage.getItem('geteat-state'));
```

### State Management
```javascript
const state = {
    currentUser: null,
    currentRoute: 'home',
    adminSettings: {
        paypalCodes: {},
        pickupPersons: {},
        orderingEnabled: {},
        adminPassword: 'admin123',
        allowedAdmins: ['administrator', 'admin', 'chef']
    },
    restaurants: [...],
    weekDays: ['Montag', 'Dienstag', 'Mittwoch', 'Donnerstag', 'Freitag'],
    votes: {},
    participants: {},
    orders: {},
    cart: {},
    orderHistory: {}
};
```

## ⚙️ Konfiguration

### Standard-Einstellungen anpassen

#### Admin-Passwort ändern
```javascript
// Im Admin Dashboard unter "Einstellungen"
// Oder direkt im Code:
adminPassword: 'dein-neues-passwort'
```

#### Erlaubte Admin-Benutzer
```javascript
allowedAdmins: ['administrator', 'admin', 'chef', 'manager']
```

#### Standard-Restaurants hinzufügen
```javascript
restaurants: [
    {
        id: 'r1',
        name: 'Restaurant Name',
        category: 'Kategorie',
        menu: [
            { id: 'm1', name: 'Gericht 1', price: 9.50 },
            { id: 'm2', name: 'Gericht 2', price: 12.00 }
        ]
    }
]
```

#### Wochentage anpassen
```javascript
weekDays: ['Montag', 'Dienstag', 'Mittwoch', 'Donnerstag', 'Freitag']
// Oder andere Sprachen/Tage
```

## 📱 Mobile Optimierung

### Responsive Features
- **Touch-optimierte Buttons** (min. 44px Höhe)
- **Mobile-freundliche Navigation** mit Burger-Menü
- **Optimierte Formulare** (16px Font-Size für iOS)
- **Swipe-Gesten** für bessere UX
- **Adaptive Layouts** für verschiedene Bildschirmgrößen

### Admin Dashboard Mobile
- **2-Spalten Tab-Layout** für bessere Navigation
- **Vollbreite Eingabefelder** für Touch-Eingabe
- **Optimierte Button-Größen** für Finger-Navigation
- **Vertikale Layouts** bei kleinen Bildschirmen

### Performance-Optimierungen
- **CSS-Animationen** statt JavaScript
- **Lazy Loading** für große Listen
- **Optimierte Event-Handler**
- **Minimale DOM-Manipulationen**

## 🔄 Datenflow

### Voting-Prozess
1. Benutzer wählt Tag aus
2. Verfügbare Restaurants werden geladen
3. Abstimmung wird gespeichert
4. Live-Update der Ergebnisse
5. Gewinner-Restaurant wird ermittelt

### Bestellprozess
1. Menü des Gewinner-Restaurants laden
2. Artikel zum Warenkorb hinzufügen
3. Bestellung aufgeben
4. PayPal-Modal anzeigen
5. Zahlungsbestätigung durch Admin

### Admin-Workflow
1. Restaurant-Management
2. Bestellungen freischalten
3. PayPal-Codes hochladen
4. Abholer zuweisen
5. Bestellungen überwachen

## 🚨 Troubleshooting

### Häufige Probleme

#### **Problem**: Bestellungen funktionieren nicht
**Lösung**: 
- Admin Dashboard öffnen
- Zu "Abholung" navigieren
- "🔓 Alle freischalten" klicken

#### **Problem**: PayPal-Modal wird nicht angezeigt
**Lösung**:
- PayPal-Code im Admin Dashboard hochladen
- Bildformat überprüfen (JPG, PNG)

#### **Problem**: Voting funktioniert nicht
**Lösung**:
- Restaurants für den Tag konfigurieren
- Mindestens 2 Restaurants auswählen

#### **Problem**: Daten gehen verloren
**Lösung**:
- Browser-Cache leeren kann Daten löschen
- Regelmäßige CSV-Exports für Backup

### Browser-Kompatibilität
```javascript
// Feature-Detection
if (typeof Storage !== "undefined") {
    // LocalStorage verfügbar
} else {
    // Fallback-Lösung
    alert("Browser unterstützt kein LocalStorage");
}
```

## 📊 Datenexport

### CSV-Export-Funktionen
- **Bestellungen CSV**: Alle Bestelldaten mit PayPal-Codes
- **Voting CSV**: Abstimmungsergebnisse pro Restaurant
- **Automatische Formatierung** für Excel/Google Sheets

### Export-Format
```csv
Tag,Benutzer,Artikel,Menge,Preis,Gesamt,PayPal Code
"Montag","Max Mustermann","Pizza Margherita",1,9.50,9.50,"paypal-code-url"
```

## 🔐 Sicherheit

### Authentifizierung
- **Admin-Passwort-Schutz**
- **Erlaubte Admin-Liste**
- **Session-basierte Anmeldung**

### Datenschutz
- **Lokale Speicherung** (keine Server-Übertragung)
- **Keine externen APIs** (außer PayPal-Bilder)
- **DSGVO-konform** durch lokale Datenhaltung

## 🎨 Anpassungen

### Design-System
```css
:root {
    --primary: #8b5cf6;
    --secondary: #06b6d4;
    --accent: #f59e0b;
    --surface: #1e293b;
    --background: #0f172a;
}
```

### Theme anpassen
- CSS Custom Properties verwenden
- Farben in `:root` definiert
- Dark/Light Mode vorbereitet

## 📈 Roadmap

### Geplante Features
- [ ] **Multi-Language Support** (EN, DE, FR)
- [ ] **Erweiterte Statistiken** mit Charts
- [ ] **Email-Benachrichtigungen**
- [ ] **Restaurant-Bewertungen**
- [ ] **Allergien/Diäten-Filter**
- [ ] **Gruppierungen** für große Teams
- [ ] **API-Integration** für externe Systeme

### Verbesserungen
- [ ] **PWA-Funktionalität** (Offline-Modus)
- [ ] **Push-Notifications** im Browser
- [ ] **Erweiterte Filteroptionen**
- [ ] **Bulk-Operationen** für Admins

## 🤝 Support

### Kontakt
- **Dokumentation**: Diese README-Datei
- **Bug Reports**: Über GitHub Issues
- **Feature Requests**: Über GitHub Discussions

### Entwicklung
- **Framework**: Vanilla JavaScript
- **Build Process**: Keine Build-Tools erforderlich
- **Development**: Direkt im Browser testbar

### Deployment
- **Statische Hosting**: Funktioniert auf jedem Webserver
- **CDN-Ready**: Alle Assets inline
- **Zero-Configuration**: Plug-and-Play

---

## 📄 Lizenz

Dieses Projekt ist unter der MIT-Lizenz lizenziert. Siehe LICENSE-Datei für Details.

## 🙏 Danksagungen

- **Icons**: Verwendet SVG-Icons für bessere Performance
- **Design**: Inspiriert von modernen Dashboard-Designs
- **UX**: Optimiert für Team-Collaboration

---

**GetEat** - Macht Team-Lunches einfach und organisiert! 🍕🥗🍜
