---
title: Перенос Exchange веб-служб (EWS) в Microsoft Graph
description: Описывает, как перенести Exchange веб-службы (EWS) в Microsoft Graph.
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 029c27940ee98b9f6b9d9077e79dc704df143e9e
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516571"
---
# <a name="migrate-exchange-web-services-ews-apps-to-microsoft-graph"></a>Перенос Exchange веб-служб (EWS) в Microsoft Graph

[Exchange Web Services (EWS)](/exchange/client-developer/exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange) — это устаревший протокол, который был в использовании Exchange Server 2007 года. В августе 2018 г. [Корпорация Майкрософт](https://techcommunity.microsoft.com/t5/exchange-team-blog/upcoming-changes-to-exchange-web-services-ews-api-for-office-365/ba-p/608055) объявила, что активных инвестиций в API EWS для Exchange Online. Настоятельно рекомендуется перенести приложения EWS, которые Exchange Online в Microsoft Graph.

## <a name="why-use-microsoft-graph"></a>Зачем использовать microsoft Graph?

Microsoft Graph предлагает улучшения по сравнению с EWS с точки зрения безопасности, простоты и эффективности. Переключение на microsoft Graph, чтобы воспользоваться этими улучшениями с помощью одной конечной точки.

### <a name="security"></a>Безопасность

Корпорация Graph майкрософт имеет более строгие политики безопасности и управления с помощью OAuth и детализации, чтобы ограничить доступ к данным в почтовом ящике в отличие от модели всех или вообще не доступных в EWS.

### <a name="developer-simplicity"></a>Простота разработчика

Microsoft Graph предлагает [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) для легкого и быстрого тестирования API, SDKs на разных языках программирования и активного сообщества разработчиков.

### <a name="rest-efficiency"></a>Эффективность REST

API Graph Майкрософт основаны на rest, где API EWS основаны на мыле. Преимущество использования протоколов на основе REST включает более быструю сериализацию JSON и более низкое использование сети.

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [различиях в](migrate-exchange-web-services-authentication.md) проверке подлинности в Microsoft Graph и EWS.
- [Просмотрите сопоставления API](migrate-exchange-web-services-api-mapping.md), чтобы найти Graph эквиваленты API EWS, которые вы используете в настоящее время.
- [Ознакомьтесь с Graph](/graph/overview) microsoft.
- Используйте [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) для экспериментов с Microsoft Graph.
