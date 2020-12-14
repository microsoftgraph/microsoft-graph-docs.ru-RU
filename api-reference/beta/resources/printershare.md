---
title: Тип ресурса printerShare
description: Представляет принтер, который должен быть обнаруживаемым пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5f8b8ad8446d37c73ddfd2b55b8ca544f1f926cd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664081"
---
# <a name="printershare-resource-type"></a>Тип ресурса printerShare

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет принтер, который должен быть обнаруживаемым пользователями и приложениями печати.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/print-list-shares.md) | [Коллекция printerShare](printershare.md) | Получите список принтеров в клиенте. |
| [получение](../api/printershare-get.md); | [printerShare](printershare.md) | Чтение свойств и связей объекта **printerShare.** |
| [Обновление](../api/printershare-update.md) | [printerShare](printershare.md) | Обновление объекта **printerShare.** |
| [удаление](../api/printershare-delete.md); | Нет | Отобрьь принтера. |
| [Список заданий](../api/printershare-list-jobs.md) | [Коллекция printJob](printjob.md) | Получите список заданий печати, которые находятся в очереди для обработки принтеромShare. |
| [Создание задания](../api/printershare-post-jobs.md) | [printJob](printjob.md) | Создайте новое задание печати для printerShare. Чтобы начать печать задания, [используйте](../api/printjob-start.md)start . |
| [Список allowedUsers](../api/printershare-list-allowedusers.md) | Коллекция объектов [user](user.md) | Получить список пользователей, которым предоставлен доступ для отправки заданий печати в связанную обойму принтера. |
| [Добавление allowedUser](../api/printershare-post-allowedusers.md) | Нет | Предодайте указанному пользователю доступ для отправки заданий печати в связанную обойму принтера. |
| [Удаление allowedUser](../api/printershare-delete-alloweduser.md) | Нет | Отозовет доступ к принтеру для доступа к данным у указанного пользователя. |
| [Список allowedGroups](../api/printershare-list-allowedgroups.md) | Коллекция [group](group.md) | Получить список групп, которые получили доступ для отправки заданий печати в связанную обойму принтера. |
| [Добавление allowedGroup](../api/printershare-post-allowedgroups.md) | Нет | Предодайте указанной группе доступ для отправки заданий печати в связанную обную долю принтера. |
| [Удаление allowedGroup](../api/printershare-delete-allowedgroup.md) | Нет | Отозовет доступ к принтеру для доступа к данным из указанной группы. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Идентификатор printerShare. Только для чтения.|
|displayName|String|Имя обоймы принтера, которую должны отображать клиенты печати.|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда была создана обойма принтера. Только для чтения.|
|manufacturer|String|Производитель, о чем сообщил принтер, связанный с этой обоймой принтером. Только для чтения.|
|model|String|Имя модели, сообщаемая принтером, связанным с этой обоймой принтером. Только для чтения.|
|isAcceptingJobs|Логический|Принимает ли принтер, связанный с этой обоймой принтера, в настоящее время принимает новые задания печати.|
|defaults|[printerDefaults](printerdefaults.md)|Параметры печати по умолчанию для принтера, связанного с этой обоймой.|
|capabilities|[printerCapabilities](printercapabilities.md)|Возможности принтера, связанного с этой обойдной частью принтера.|
|расположение|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение принтера, связанного с этой обоймой принтера.|
|status|[printerStatus](printerstatus.md)|Состояние обработки, включая все ошибки, принтера, связанного с этой обоймой принтера. Только для чтения.|
|allowAllUsers|Логический|Если задана истина, всем пользователям и группам будет предоставлен доступ к этой обойме принтера. Это замеает списки разрешенных, определенные свойствами **навигации allowedUsers** и **allowedGroups.**|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|printer|[printer](printer.md)|Принтер, с который связан этот принтер. |
|allowedUsers|Коллекция объектов [user](user.md)|Пользователи, у которых есть доступ к печати с помощью принтера.|
|allowedGroups|[group](group.md)|Группы, пользователи которых имеют доступ к печати с помощью принтера.|
|jobs|[Коллекция printJob](printjob.md)| Список заданий, которые находятся в очереди для печати принтером, связанным с этой обоймой принтера.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "createdDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


