# Web application packaging

## core

- apllication
  - exception
  - service
- domain
  - fundamentals
  - model
- infrastructure
  - search
  - aws
  - datadource
  - image
- presentation
  - exception
  - ogp
  - seo

## application-core
- domain
  - fundamentals
  - model
  - validation
  - service

## app-batch
- 上に同じ

## app-ui
- presentation
  - controller
    - advice
      - PagenationAdvice.java
      - ExceptionAdvice.java
      - BinderAdvice.java
      - LocaleAdvice.java
  - view
    - error
    - api
    - request
    - response

## database
- migration

# 各種

### application層
- 例外処理層
- サービス層

### domain層
- 業務の関心事

### infrastructure層
- Database層
- 外部サービス連携層

### presentation層
- プレゼンテーションの関心事を格納する
 - Controller層(フロントエンドとの連携モジュール)
 - パンくず(パンくずもフロントと直結する。)
 - SEO(SEOもUIとフロントと直結する)
   - ロボット
   - TDK
 - ページャー(ページャーもフロントと直結する)