# RiotAPI [![Build Status](https://travis-ci.org/ejeong0915/RiotAPI.svg?branch=master)](https://travis-ci.org/ejeong0915/RiotAPI)

## Get Started

...
...

## Description
...
...

## Usage
...
...

## Api Endpoints and Calls
###### Note: All Endpoints and Objects are based on the documentation https://developer.riotgames.com/api-methods/
#### Endpoint: ChampionMasteryV3
Call | Parameters | Return
---- | ---------- | ------
getMasteries() | string $region, int $summonerId | Array[ChampionMastery]
getMasteryByChampion() | string $region, int $summonerId, int $championId | ChampionMastery
getScore() | string $region, int $summonerId | int

#### Endpoint: ChampionV3
Call | Parameters | Return
---- | ---------- | ------
getChampions() | string $region | Array[Champion]
getChampionById() | string $region, int $championId | Champion

#### Endpoint: LeagueV3
Call | Parameters | Return
---- | ---------- | ------
getChallengerLeague() | string $region, string $queue | LeagueList
getLeagueById() | string $region, string $leagueId | LeagueList
getMasterLeague() | string $region, string $queue | LeagueList
getAllLeaguePositionsForSummoner() | string $region, int $summonerId | Array[LeaguePosition]

#### Endpoint: LoLStaticDataV3 (in progress)
###### Note: Parameters are optional parameters in the api like 'version' or 'tags'
Call | Parameters | Return
---- | ---------- | ------
getChampions() | not implemented | not implemented
getChampionById() | not implemented | not implemented
getItems() | not implemented | not implemented
getItemById() | string $region, int $id, array $parameters | Item
getLanguageStrings() | string $region, array $parameters | LanguageStrings
getLanguages() | string $region | Array[string]
getMaps() | string $region, array $parameters | MapData
getMasteries() | not supported | request if needed
getMasteryById() | not supported | request if needed
getProfileIcons() | string $region, array $parameters | ProfileIconData
getRealms() | string $region | Realm
getRunes() | not supported | request if needed
getRuneById() | not supported | request if needed
getSummonerSpells() | string $region, array $parameters | SummonerSpellList
getSummonerSpellById() | string $region, int $id, array $parameters | SummonerSpell
getVersions() | string $region | Array[string]

#### Endpoint: LoLStatusV3
Call | Parameters | Return
---- | ---------- | ------
getStatus() | string $region | ShardData

#### Endpoint: MatchV3 (not implemented)
Call | Parameters | Return
---- | ---------- | ------
getMatch() | not implemented | not implemented
getMatchlist() | not implemented | not implemented
getRecentMatchlist() | not implemented | not implemented
getMatchTimeline() | not implemented | not implemented
getMatchIdsByTournamentCode() | not implemented | not implemented
getMatchByTournamentCode() | not implemented | not implemented

#### Endpoint: SpectatorV3
Call | Parameters | Return
---- | ---------- | ------
getCurrentGameInfoBySummoner() | string $region, int $summonerId | CurrentGameInfo
getFeaturedGames() | string $region | FeaturedGames

#### Endpoint: SummonerV3
Call | Parameters | Return 
---- | ---------- | ------
getSummonerById() | string $region, int $id | Summoner
getSummonerByAccountId() | string $region, int $id | Summoner
getSummonerByName() | string $region, string $name | Summoner

#### Endpoint: ThirdPartyCodeV3
Call | Parameters | Return
---- | ---------- | ------
getBySummonerId() | string $region, int $summonerId | string
