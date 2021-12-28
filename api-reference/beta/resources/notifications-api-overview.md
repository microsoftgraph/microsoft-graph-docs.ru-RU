---
title: Использование REST API уведомлений в Microsoft Graph (не рекомендуется)
description: Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph.
ms.localizationpriority: high
ms.prod: notifications
doc_type: conceptualPageType
author: merzink
ms.openlocfilehash: 2c235bfa383238897efa5d55f58f4a97865e3e56
ms.sourcegitcommit: 7a0f9f1a535795c6f77c80e02fd97581c36f1273
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/27/2021
ms.locfileid: "61609034"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph-deprecated"></a>Использование REST API уведомлений в Microsoft Graph (не рекомендуется)

> [!IMPORTANT]
> API уведомлений Microsoft Graph не рекомендуется и прекратит возвращать данные к концу января 2022 г. Дополнительные сведения см. в [Центрах уведомлений Microsoft Azure](/azure/notification-hubs) и в [этой записи блога](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/).  

Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто отправьте уведомление целевому пользователю, и платформа доставит его во все конечные точки устройств, зарегистрированные для этого пользователя. На высоком уровне процесс выглядит так:

1. Пользователь входит в приложение, которое создает подписку в службе уведомлений Microsoft Graph. Приложению, отправившему вызов, будет возвращен конкретный идентификатор подписки на уведомления пользователя, или UNSID.
2. Приложение отправляет этот UNSID в службу приложений.
3. Когда служба приложений будет готова отправить уведомление, она [проходит проверку подлинности на платформе удостоверений Майкрософт](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) и отправляет уведомление через службу уведомлений Microsoft Graph, предоставляя маркер проверки подлинности, UNSID целевого пользователя и полезные данные уведомления.
4. Служба уведомлений Microsoft Graph рассылает уведомления всем конечным точкам пользователя с активной подпиской.

Уведомления такого типа, ориентированные на пользователя, представлены ресурсом [notification](../resources/projectrome-notification.md) и хранятся в службе уведомлений Microsoft Graph. Доступ к нему и управление осуществляется клиентским приложением с помощью [клиентских API SDK](https://aka.ms/GNSDK). Если вы впервые работаете со службой уведомлений Microsoft Graph, ознакомьтесь с дополнительными сведениями в разделе [обзора уведомлений](/graph/notifications-concept-overview).

## <a name="next-steps"></a>Дальнейшие действия

- См. статью [Ресурс notification](../resources/projectrome-notification.md) и создавайте уведомления для взаимодействия с пользователями.
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Приступите к интеграции клиента, следуя инструкциями из [обзора интеграции](/graph/notifications-integration-e2e-overview).