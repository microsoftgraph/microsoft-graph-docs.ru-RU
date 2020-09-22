---
title: Использование REST API уведомлений в Microsoft Graph
description: Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. .
localization_priority: Priority
ms.prod: notifications
doc_type: conceptualPageType
author: merzink
ms.openlocfilehash: 96b27aa9a57c26666ae9b4fc09c4dadca52b8d6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033659"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Использование REST API уведомлений в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто отправьте уведомление целевому пользователю, и платформа доставит его во все конечные точки устройств, зарегистрированные для этого пользователя. На высоком уровне процесс выглядит так:

1. Пользователь входит в приложение, которое создает подписку в службе уведомлений Microsoft Graph. Приложению, отправившему вызов, будет возвращен конкретный идентификатор подписки на уведомления пользователя, или UNSID.
2. Приложение отправляет этот UNSID в службу приложений.
3. Когда служба приложений будет готова отправить уведомление, она [проходит проверку подлинности на платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) и отправляет уведомление через службу уведомлений Microsoft Graph, предоставляя маркер проверки подлинности, UNSID целевого пользователя и полезные данные уведомления.
4. Служба уведомлений Microsoft Graph рассылает уведомления всем конечным точкам пользователя с активной подпиской.  

Уведомления такого типа, ориентированные на пользователя, представлены ресурсом [notification](../resources/projectrome-notification.md) и хранятся в службе уведомлений Microsoft Graph. Доступ к нему и управление осуществляется клиентским приложением с помощью [клиентских API SDK](https://aka.ms/GNSDK). Если вы впервые работаете со службой уведомлений Microsoft Graph, ознакомьтесь с дополнительными сведениями в разделе [обзора уведомлений](https://docs.microsoft.com/graph/notifications-concept-overview).    

## <a name="whats-new"></a>Что нового
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия
- См. статью [Ресурс notification](../resources/projectrome-notification.md) и создавайте уведомления для взаимодействия с пользователями. 
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Приступите к интеграции клиента, следуя инструкциями из [обзора интеграции](/graph/notifications-integration-e2e-overview).


