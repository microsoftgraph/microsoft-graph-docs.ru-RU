---
title: Использование REST API уведомлений в Microsoft Graph
description: Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства. Запросы API уведомлений выполняются от имени пользователя посредством делегированных разрешений и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 28aa795b1df9b2f4817c69332dd8bc9bf3afb172
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422523"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Использование REST API уведомлений в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства. Запросы API уведомлений выполняются от имени пользователя посредством [делегированных разрешений](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.
Этот тип уведомления, ориентированного на пользователя, представлен ресурсом [notification](../resources/projectrome-notification.md) и хранится в Microsoft Graph. Доступ к нему и управление можно обеспечить путем публикации приложения с помощью [клиентских API SDK](https://github.com/Microsoft/project-rome). 

## <a name="next-steps"></a>Дальнейшие действия
- См. статью [Ресурс notification](../resources/projectrome-notification.md) и создавайте уведомления для взаимодействия с пользователями. 
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Начните работу с использованием интеграции с клиентом, следуя инструкциям, указанным в [обзоре интеграции](/graph/notifications-integration-e2e-overview).
