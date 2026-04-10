# Gocyclo Summary

Source: `.codex-reports/gocyclo-all.txt`

## Coverage

- Go files scanned: 214
- Functions and methods measured: 1605
- Functions and methods in non-`*_test.go` files: 847
- Overall average complexity: 2.70
- Non-`*_test.go` average complexity: 2.62
- Overall median complexity: 2
- Non-`*_test.go` median complexity: 2
- Overall max complexity: 19 in `TestMarketPositionsHandlerWithService_IncludesZeroPositionUsers` at `backend/handlers/positions/positionshandler_test.go:103:1`
- Non-`*_test.go` max complexity: 12 in `containsMaliciousDomain` at `backend/security/sanitizer.go:299:1`

## Threshold Counts

- Overall functions with complexity >= 15: 6
- Overall functions with complexity >= 12: 15
- Overall functions with complexity >= 10: 29
- Overall functions with complexity >= 8: 80
- Non-`*_test.go` functions with complexity >= 15: 0
- Non-`*_test.go` functions with complexity >= 12: 1
- Non-`*_test.go` functions with complexity >= 10: 4
- Non-`*_test.go` functions with complexity >= 8: 23

## Top 15 Overall

- 19 `TestMarketPositionsHandlerWithService_IncludesZeroPositionUsers` `backend/handlers/positions/positionshandler_test.go:103:1`
- 18 `TestGetPublicResponseMarketMapping` `backend/handlers/marketpublicresponse/publicresponsemarket_test.go:86:1`
- 18 `TestComputeSystemMetrics_BalancedAfterFinalLockedBet` `backend/internal/domain/analytics/systemmetrics_integration_test.go:42:1`
- 15 `TestMarketBetsHandlerWithService` `backend/handlers/bets/betshandler_test.go:72:1`
- 15 `TestSeedHomepage_Integration_WithActualFile` `backend/seed/integration_test.go:13:1`
- 15 `TestSeedHomepage_RendersHTML` `backend/seed/seed_test.go:12:1`
- 14 `TestMarketGate_Open` `backend/internal/domain/bets/service_helpers_test.go:104:1`
- 14 `TestServiceGetUserPortfolio` `backend/internal/domain/users/service_transactions_test.go:121:1`
- 13 `TestListUserMarketsReturnsDistinctMarketsOrderedByRecentBet` `backend/handlers/users/listusers_test.go:16:1`
- 13 `TestResolveMarket_DistributesAllBetVolume` `backend/internal/domain/analytics/systemmetrics_integration_test.go:144:1`
- 13 `TestServiceSell_Succeeds` `backend/internal/domain/bets/service_test.go:411:1`
- 13 `TestRun_AppliesInOrder_And_Persists` `backend/migration/migrate_test.go:33:1`
- 12 `TestUserMarketPositionHandlerReturnsUserPosition` `backend/handlers/users/userpositiononmarkethandler_test.go:21:1`
- 12 `TestGormRepositoryListBetsForMarket` `backend/internal/repository/markets/repository_test.go:84:1`
- 12 `containsMaliciousDomain` `backend/security/sanitizer.go:299:1`

## Top 15 In Non-*_test.go Files

- 12 `containsMaliciousDomain` `backend/security/sanitizer.go:299:1`
- 11 `(MarketShareCalculator).withDefaults` `backend/internal/domain/math/outcomes/dbpm/marketshares.go:199:1`
- 11 `(*Service).GetUserPortfolio` `backend/internal/domain/users/service.go:392:1`
- 10 `TestMarketTitleValidation` `backend/handlers/markets/createmarket_test_security.go:9:1`
- 9 `TestMarketDescriptionValidation` `backend/handlers/markets/createmarket_test_security.go:86:1`
- 9 `(saleCalculator).Calculate` `backend/internal/domain/bets/bet_sell.go:74:1`
- 8 `processAddUser` `backend/handlers/admin/adduser.go:45:1`
- 8 `(*Service).UpdateHome` `backend/handlers/cms/homepage/service.go:104:1`
- 8 `TestMarketInputXSSPrevention` `backend/handlers/markets/createmarket_test_security.go:167:1`
- 8 `(*Handler).ResolveMarket` `backend/handlers/markets/handler.go:243:1`
- 8 `(*Handler).parseSearchParams` `backend/handlers/markets/handler.go:570:1`
- 8 `(*Service).ComputeUserFinancials` `backend/internal/domain/analytics/financials.go:9:1`
- 8 `(*Service).ComputeGlobalLeaderboard` `backend/internal/domain/analytics/leaderboard.go:25:1`
- 8 `(*Service).Sell` `backend/internal/domain/bets/bet_sell.go:10:1`
- 8 `(*Service).GetMarketLeaderboard` `backend/internal/domain/markets/market_leaderboard.go:11:1`

## Top 10 Non-*_test.go Files By Aggregate Complexity

- `backend/internal/domain/users/service.go` total=154 max=11 symbols=50
- `backend/security/sanitizer.go` total=92 max=12 symbols=22
- `backend/handlers/markets/handler.go` total=89 max=8 symbols=19
- `backend/internal/domain/math/outcomes/dbpm/marketshares.go` total=86 max=11 symbols=41
- `backend/internal/domain/markets/service_policies.go` total=79 max=7 symbols=29
- `backend/internal/repository/markets/repository.go` total=66 max=6 symbols=24
- `backend/internal/domain/analytics/repository.go` total=56 max=7 symbols=19
- `scripts/seed_markets.go` total=52 max=8 symbols=12
- `backend/internal/domain/markets/service.go` total=50 max=2 symbols=30
- `backend/internal/domain/bets/service.go` total=47 max=2 symbols=28
