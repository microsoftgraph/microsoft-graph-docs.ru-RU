---
title: Перенос Exchange веб-служб (EWS) в Microsoft Graph
description: Описывается, как перенести Exchange веб-служб (EWS) в Microsoft Graph.
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: dcc9d75e82fa2a6b09298a8b5068f2c55e2a8be4
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549605"
---
# <a name="migrate-exchange-web-services-ews-apps-to-microsoft-graph"></a>Перенос Exchange веб-служб (EWS) в Microsoft Graph

[Exchange Веб-службы (EWS)](/exchange/client-developer/exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange) — это устаревший протокол, который используется с Exchange Server 2007 года. В августе 2018 г. корпорация [Майкрософт](https://techcommunity.microsoft.com/t5/exchange-team-blog/upcoming-changes-to-exchange-web-services-ews-api-for-office-365/ba-p/608055) объявила о том, что не будет никаких активных инвестиций в API EWS для Exchange Online. Настоятельно рекомендуется перенести приложения EWS, которые Exchange Online в Microsoft Graph.

## <a name="why-use-microsoft-graph"></a>Зачем использовать Microsoft Graph?

Microsoft Graph предлагает улучшения по сравнению с EWS с точки зрения безопасности, простоты и эффективности. Перейдите на Graph Майкрософт, чтобы воспользоваться преимуществами этих улучшений с помощью одной конечной точки.

### <a name="security"></a>Безопасность

Microsoft Graph имеет более строгие политики безопасности и управления с помощью OAuth и детализированное определение области, чтобы ограничить доступ к данным в почтовом ящике, в отличие от модели доступа "все" или "нет" в EWS.[](/graph/permissions-reference)

### <a name="developer-simplicity"></a>Простота разработчика

Microsoft Graph [предлагает Graph Explorer для](https://developer.microsoft.com/graph/graph-explorer) легкого и быстрого обнаружения и тестирования API, [пакетов SDK](/graph/sdks/sdks-overview) на разных языках программирования и активного сообщества разработчиков.

### <a name="rest-efficiency"></a>Эффективность REST

Microsoft Graph API основаны на REST, где API EWS основаны на SOAP. Преимущество использования протоколов на основе REST заключается в более быстрой сериализации JSON и снижении использования сети.

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [различиях в проверке](migrate-exchange-web-services-authentication.md) подлинности в Microsoft Graph и EWS.
- [Просмотрите сопоставления API](migrate-exchange-web-services-api-mapping.md), чтобы найти Graph майкрософт для API EWS, которые вы используете в настоящее время.
- [Изучите Graph](/graph/overview) и методики Майкрософт.
- Используйте [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) для экспериментов с Microsoft Graph.
