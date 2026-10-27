# Netwerk, DNS en HTTPS

Week 26 okt – 1 nov. Doel: uitleggen wat er gebeurt tussen het intypen van een adres en het zien van de pagina.

Draai de commando's in Azure Cloud Shell (PowerShell) en schrijf onder elk commando in één zin wat je zag.

## Het verhaal in 5 stappen

Ezelsbrug: **Dikke Taxi's Hebben Altijd Antwoord**

1. **D**NS: welk IP-adres hoort bij de naam?
2. **T**CP: verbinding met dat IP op poort 443.
3. **H**andshake (TLS): certificaat tonen en controleren, sleutel afspreken.
4. **A**anvraag (HTTP): de browser vraagt versleuteld om de pagina.
5. **A**ntwoord: HTML terug met een statuscode (200, 404, 500).

## 1. DNS: naam naar IP

```bash
nslookup bit-academy.nl
```

Wat ik zag:

```bash
dig bit-academy.nl A +short
```

Wat ik zag:

## 2. CNAME-keten

```bash
dig www.microsoft.com CNAME
```

Wat ik zag:

## 3. HTTP-headers

```bash
curl -I https://bit-academy.nl
```

Wat ik zag:

## 4. TLS-handshake en certificaat

```bash
curl -v https://bit-academy.nl -o /dev/null
```

Wat ik zag:

## In mijn eigen woorden

Wat gebeurt er als ik `https://bit-academy.nl` intyp? Koppel elke stap aan een commando hierboven.

