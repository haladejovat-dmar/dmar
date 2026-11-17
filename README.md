# D’MAR – aktualizovaný web pro GitHub Pages (10. 11. 2026)

Nahrát obsah ZIPu do kořene GitHub repozitáře. `index.html` je vstupní stránka.

## Potvrzeno
- Ing. Tereza Haladějová, IČO 30198411, sídlo Jistebník 230, 742 82 Jistebník
- info@dmar.cz, +420 775 916 369
- doprava Zásilkovna/Packeta ČR a Slovensko
- doprava zdarma při hodnotě zboží od 3 000 Kč
- platební karta, expedice do 3 pracovních dnů od přijetí platby, hotové zboží
- vrácení na adresu sídla, dopravu u odstoupení bez vady hradí zákazník

## Napojení na Shopify (17. 11. 2026)
- Web zůstává na GitHub Pages; Shopify slouží jen jako pokladna.
- Fotky se načítají ze Shopify CDN (index.html má 0,3 MB místo 4,6 MB).
- Každá kabelka má v `products` pole `variantId` (ID varianty v Shopify) a `handle`.
- Košík se ukládá v prohlížeči; tlačítko „Pokračovat k pokladně“ vede na
  `https://cahxyu-j6.myshopify.com/cart/<variantId>:1,...` (konstanta `DMAR_SHOP`).
- Nová kabelka: založit v Shopify, pak doplnit do `products` včetně `variantId`.
- Prodaná kabelka: Shopify ji sám nepustí znovu koupit; na webu nastavit `stock:0`.

## DŮLEŽITÉ
- Navrhované ceny zákaznické dopravy: ČR výdejní místo 99 Kč, SK výdejní místo 119 Kč. Jde o návrh D’MAR, NE ověřený závazný firemní ceník Zásilkovny.
- Cena a dostupnost dalších služeb Zásilkovny, Packeta aplikace, skutečné produkty, DPH/OSS pro zahraniční dodávky, GDPR/cookies a právní kontrola se dokončí před spuštěním.
