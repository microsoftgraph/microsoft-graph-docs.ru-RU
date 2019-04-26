---
title: Использование REST API уведомлений в Microsoft Graph
description: Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства. Запросы API уведомлений выполняются от имени пользователя посредством делегированных разрешений и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 243f412162ed1427c766272d02d58c57ba47cf42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342102"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Использование REST API уведомлений в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства. Запросы API уведомлений выполняются от имени пользователя посредством [делегированных разрешений](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.
Этот тип уведомления, ориентированного на пользователя, представлен ресурсом [notification](../resources/projectrome-notification.md) и хранится в Microsoft Graph. Доступ к нему и управление можно обеспечить путем публикации приложения с помощью [API SDK Project Rome](https://github.com/Microsoft/project-rome). 

## <a name="next-steps"></a>Дальнейшие действия
- См. статью [Ресурс notification](../resources/projectrome-notification.md) и создавайте уведомления для взаимодействия с пользователями. 
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
