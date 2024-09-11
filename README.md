# Optimierte Preisanzeige für Shopify

Diese Anleitung erklärt, wie Sie eine optimierte Preisanzeige in Ihr Shopify-Theme integrieren können.

## Funktionen

- Anzeige des aktuellen Preises
- Anzeige des ursprünglichen Preises (falls im Angebot)
- Prozentuale Ersparnis-Anzeige
- "Angebot"-Label
- "Ausverkauft"-Badge
- Responsive Design

## Integration

### 1. Erstellen Sie ein neues Snippet

- Erstellen Sie eine neue Datei `snippets/price.liquid` in Ihrem Shopify-Theme.
- Kopieren Sie den Code aus der bereitgestellten `price.liquid`-Datei in dieses neue Snippet.

### 2. Verwendung des Snippets

Um die optimierte Preisanzeige zu verwenden, fügen Sie folgenden Code an der gewünschten Stelle in Ihren Theme-Dateien ein:

```liquid
{% render 'price', product: product, use_variant: true %}
```

### 3. Anpassungsmöglichkeiten

- `product`: Das Produkt-Objekt, für das der Preis angezeigt werden soll.
- `use_variant`: Wenn auf `true` gesetzt, wird der Preis der ausgewählten oder ersten verfügbaren Variante angezeigt.
- `show_badges`: Wenn auf `true` gesetzt, werden "Angebot" und "Ausverkauft" Badges angezeigt.

### 4. Styling

Das Snippet enthält bereits integriertes CSS für das Styling. Sie können dies nach Bedarf in Ihrer Theme-Datei anpassen.

## Beispiel-Ausgabe

Die Preisanzeige kann je nach Produktstatus unterschiedlich aussehen:

1. Normaler Preis
2. Angebotspreis mit Ersparnis
3. Ausverkauft

## Anpassungen

Sie können das Aussehen der Preisanzeige anpassen, indem Sie den CSS-Code im `<style>`-Abschnitt des Snippets bearbeiten.

## Unterstützung

Bei Fragen oder Problemen öffnen Sie bitte ein Issue in diesem Repository.
