# Pokémon TCG API (pokemon-tcg)

The Pokémon TCG API is a free, community-run REST API created and maintained by Andrew Backes that serves Pokémon Trading Card Game data - more than 20,000 cards across 170+ sets, from Base Set onward. Every card carries full gameplay data (attacks, abilities, weaknesses, resistances, retreat costs), format legalities, high-resolution card images, and daily-updated market prices from TCGplayer and Cardmarket. A Lucene-like query syntax supports keyword, phrase, wildcard, exact, range, and nested-field searches across every field. The API works without authentication at a reduced rate limit; a free API key from the developer portal, sent in the `X-Api-Key` header, raises the limits. Official SDKs cover Python, Ruby, JavaScript, TypeScript, C#, Kotlin, PHP, Go, Dart, and Elixir. It is an independent community project sustained by Patreon and Ko-fi donations, and is not produced, endorsed, or affiliated with Nintendo or The Pokémon Company.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/apis.yml)

## Tags

- Pokemon
- Trading Cards
- TCG
- Gaming
- Card Games
- Collectibles
- Card Prices

## Timestamps

- **Created:** 2026-07-11
- **Modified:** 2026-07-11

## APIs

### Pokémon TCG Cards API

Search and retrieve individual Pokémon, Trainer, and Energy cards. Each card includes gameplay data (HP, attacks, abilities, weaknesses, resistances, retreat cost), rarity, artist, flavor text, National Pokédex numbers, format legalities, small and hi-res card images, and daily-updated TCGplayer and Cardmarket prices. Supports Lucene-like queries, ordering, field selection, and pagination up to 250 cards per page.

- **Human URL:** [https://docs.pokemontcg.io/api-reference/cards/search-cards](https://docs.pokemontcg.io/api-reference/cards/search-cards)
- **Base URL:** `https://api.pokemontcg.io/v2`

#### Tags

- Pokemon
- Cards
- Trading Cards
- Card Prices

#### Properties

- [Documentation](https://docs.pokemontcg.io/api-reference/cards/card-object)
- [API Reference](https://docs.pokemontcg.io/api-reference/cards/search-cards)
- [OpenAPI](openapi/pokemon-tcg-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pokemon-tcg.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pokemon-tcg.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pokémon TCG Sets API

Search and retrieve trading card game sets (expansions) - Base Set through the latest series - with printed and total card counts, series grouping, release dates, Pokémon TCG Online/Live codes, format legalities, and set symbol and logo images. Uses the same query, ordering, selection, and pagination parameters as the Cards API.

- **Human URL:** [https://docs.pokemontcg.io/api-reference/sets/search-sets](https://docs.pokemontcg.io/api-reference/sets/search-sets)
- **Base URL:** `https://api.pokemontcg.io/v2`

#### Tags

- Pokemon
- Sets
- Expansions
- TCG

#### Properties

- [Documentation](https://docs.pokemontcg.io/api-reference/sets/set-object)
- [API Reference](https://docs.pokemontcg.io/api-reference/sets/search-sets)
- [OpenAPI](openapi/pokemon-tcg-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pokemon-tcg.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pokemon-tcg.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Pokémon TCG Metadata API

The controlled vocabularies used across the card catalog - the eleven energy types (Fire, Water, Grass, Lightning, and the rest), forty card subtypes (Basic, Stage 1, EX, GX, V, VMAX, TAG TEAM, Item, Supporter, Stadium, and more), the three supertypes (Energy, Pokémon, Trainer), and all card rarities. Useful for building search filters and validating queries against the Cards and Sets APIs.

- **Human URL:** [https://docs.pokemontcg.io/api-reference/types/get-types](https://docs.pokemontcg.io/api-reference/types/get-types)
- **Base URL:** `https://api.pokemontcg.io/v2`

#### Tags

- Pokemon
- Types
- Rarities
- Reference Data

#### Properties

- [Documentation](https://docs.pokemontcg.io/api-reference/types/get-types)
- [API Reference](https://docs.pokemontcg.io/api-reference/rarities/get-rarities)
- [OpenAPI](openapi/pokemon-tcg-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pokemon-tcg.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pokemon-tcg.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Access Model

The Pokémon TCG API is completely free to use. No payment tier exists:

- **Without an API key** - anonymous requests are limited to 1,000 requests/day and a maximum of 30 requests/minute.
- **With a free API key** - sign up at the [Pokémon TCG Developer Portal](https://dev.pokemontcg.io) and send the key in the `X-Api-Key` header for a default limit of 20,000 requests/day; higher limits can be requested via Discord or email.

The project is funded by community donations ([Patreon](https://www.patreon.com/pokemon_tcg_api) / Ko-fi), not by charging for access.

## Common Properties

- [Website](https://pokemontcg.io)
- [Documentation](https://docs.pokemontcg.io)
- [GitHub Organization](https://github.com/PokemonTCG)
- [Portal Signup](https://dev.pokemontcg.io)
- [SDKs](https://docs.pokemontcg.io/sdks/overview)
- [Rate Limits Documentation](https://docs.pokemontcg.io/getting-started/rate-limits)
- [Authentication](https://docs.pokemontcg.io/getting-started/authentication)
- [Errors](https://docs.pokemontcg.io/getting-started/errors)
- [Plans](plans/pokemon-tcg-plans-pricing.yml)
- [Rate Limits](rate-limits/pokemon-tcg-rate-limits.yml)
- [Fin Ops](finops/pokemon-tcg-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
