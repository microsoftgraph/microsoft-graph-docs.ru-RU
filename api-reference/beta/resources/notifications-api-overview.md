---
title: Использование REST API уведомлений в Microsoft Graph
description: Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства. Запросы API уведомлений выполняются от имени пользователя посредством делегированных разрешений и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 2a4c23955e348159d2e17514d6041260f13cffba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513986"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Использование REST API уведомлений в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для отправки push-уведомлений пользователю можно использовать API уведомлений в Microsoft Graph. Просто укажите учетную запись пользователя для отправки уведомления, и платформа доставит уведомление во все конечные точки устройства. Запросы API уведомлений выполняются от имени пользователя посредством [делегированных разрешений](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) и [разрешения на уведомления]( /graph/permissions_reference), которые можно использовать с учетными записями Майкрософт, рабочими или учебными учетными записями.
Этот тип уведомления, ориентированного на пользователя, представлен ресурсом [notification](../resources/projectrome-notification.md) и хранится в Microsoft Graph. Доступ к нему и управление можно обеспечить путем публикации приложения с помощью [API SDK Project Rome](https://github.com/Microsoft/project-rome). 

## <a name="next-steps"></a>Дальнейшие действия
- См. статью [Ресурс notification](../resources/projectrome-notification.md) и создавайте уведомления для взаимодействия с пользователями. 
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/notifications-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
