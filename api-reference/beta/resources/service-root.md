---
title: Корневой каталог для обслуживания
description: 2015-10-25 14:57:30 UTC-->
localization_priority: Normal
ms.openlocfilehash: 5e9c464c50dcbef7a03ca3a2fc2b0aaac40fbb30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524312"
---
# <a name="service-root"></a>Корневой каталог для обслуживания

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>Методы



| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание устройства](../api/device-post-devices.md) |[device](device.md)| Создание устройства путем добавления в коллекцию устройств.|
|[Список устройств](../api/device-list.md) | Коллекция объектов [device](device.md) |Получение коллекции объектов device. |
|[Активация directoryRole](../api/directoryrole-post-directoryroles.md) | [directoryRole](directoryrole.md) |Активация роли каталога. |
|[Список объектов directoryRole](../api/directoryrole-list.md) | Коллекция объектов [directoryRole](directoryrole.md) |Получение коллекции объектов directoryRole. |
|[Список объектов directoryRoleTemplate](../api/directoryroletemplate-list.md) | Коллекция объектов [directoryRoleTemplate](directoryroletemplate.md) |Получение коллекции объектов directoryRoleTemplate. |
|[Список дисков](../api/drive-list.md) | Коллекция объектов [drive](drive.md) |Получение коллекции объектов drive. |
|[Получение диска](../api/drive-get.md) | [drive](drive.md)  |Получение свойств объекта drive. |
|[Создание группы](../api/group-post-groups.md) |[group](group.md)| Создание группы путем добавления в коллекцию групп.|
|[Список групп](../api/group-list.md) | Коллекция объектов [group](group.md) |Получение коллекции объектов group. |
|[Список организаций](../api/organization-list.md) | Коллекция объектов [organization](organization.md) |Получение коллекции объектов organization. |
|[Список объектов subscribedSku](../api/subscribedsku-list.md) | Коллекция объектов [subscribedSku](subscribedsku.md) |Получение коллекции объектов subscribedSku. |
|[Создание пользователя](../api/user-post-users.md) |[user](user.md)| Создание пользователя путем добавления в коллекцию пользователей.|
|[Список пользователей](../api/user-list.md) | Коллекция объектов [user](user.md) |Получение коллекции объектов user. |
|[Создание connectorGroup](../api/connectorgroup-post-connectorgroups.md) |[connectorGroup](connectorgroup.md)|Создайте новый connectorGroup, отправку сообщений в коллекцию connectorGroups.|
|[Список connectorGroup](../api/connectorgroup-list.md) | [connectorGroup](connectorgroup.md) коллекции |Получите коллекцию объектов connectorGroup. |
|[Список соединителей](../api/connector-list.md) | Коллекция [соединителей](connector.md) |Получите коллекцию объектов соединителя. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/service-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
