---
title: Перенос приложений веб-служб Exchange (EWS) в Microsoft Graph
description: Так как активных инвестиций в API EWS для Exchange Online больше нет, вы можете перенести приложения EWS, которые Exchange Online в Microsoft Graph.
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 53fb8e4df5a5211fb275dde9d2b646459b63dfc2
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577730"
---
# <a name="migrate-exchange-web-services-ews-apps-to-microsoft-graph"></a>Перенос приложений веб-служб Exchange (EWS) в Microsoft Graph

[Веб-службы Exchange (EWS)](/exchange/client-developer/exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange) — это устаревший протокол, который используется с Exchange Server 2007 года. В августе 2018 г. корпорация [Майкрософт](https://techcommunity.microsoft.com/t5/exchange-team-blog/upcoming-changes-to-exchange-web-services-ews-api-for-office-365/ba-p/608055) объявила о том, что не будет никаких активных инвестиций в API EWS для Exchange Online. Настоятельно рекомендуется перенести приложения EWS, которые Exchange Online в Microsoft Graph.

## <a name="why-use-microsoft-graph"></a>Зачем использовать Microsoft Graph?

Microsoft Graph предлагает улучшения по сравнению с EWS с точки зрения безопасности, простоты и эффективности. Перейдите в Microsoft Graph, чтобы воспользоваться преимуществами этих улучшений с помощью одной конечной точки.

### <a name="security"></a>Безопасность

Microsoft Graph имеет более строгие политики безопасности и управления с OAuth и [](/graph/permissions-reference) детализированное определение области для ограничения доступа к данным в почтовом ящике в отличие от модели доступа "все" или "нет" в EWS.

### <a name="developer-simplicity"></a>Простота разработчика

Microsoft Graph предлагает [Песочницу Graph](https://developer.microsoft.com/graph/graph-explorer) для легкого и быстрого обнаружения и тестирования API, [пакетов SDK](/graph/sdks/sdks-overview) на разных языках программирования и активного сообщества разработчиков.

### <a name="rest-efficiency"></a>Эффективность REST

API Microsoft Graph основаны на REST, где API EWS основаны на SOAP. Преимущество использования протоколов на основе REST заключается в более быстрой сериализации JSON и снижении использования сети.

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [различиях в проверке подлинности](migrate-exchange-web-services-authentication.md) в Microsoft Graph и EWS.
- [Просмотрите сопоставления API](migrate-exchange-web-services-api-mapping.md), чтобы найти эквиваленты Microsoft Graph для API EWS, которые вы используете в настоящее время.
- [Изучите основные](/graph/overview) понятия и методики Microsoft Graph.
- Используйте [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer) для экспериментов с Microsoft Graph.
