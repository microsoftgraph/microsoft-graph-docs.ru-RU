---
title: Тип ресурса printerShare
description: Представляет принтер, который предназначен для обнаружения пользователями и приложениями печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ab0dbf8ff2e7a8e64f51cf72afec5415bec265e6
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176684"
---
# <a name="printershare-resource-type"></a>Тип ресурса printerShare

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет принтер, который предназначен для обнаружения пользователями и приложениями печати.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/print-list-shares.md) | [Коллекция printerShare](printershare.md) | Получение списка общих папок принтера в клиенте. |
| [получение](../api/printershare-get.md); | [printerShare](printershare.md) | Чтение свойств и связей объекта **printerShare** . |
| [Обновление](../api/printershare-update.md) | [printerShare](printershare.md) | Обновление объекта **printerShare** . |
| [удаление](../api/printershare-delete.md); | Нет | Отмените общий доступ к принтеру. |
| [Список заданий](../api/printershare-list-jobs.md) | [Коллекция printJob](printjob.md) | Получение списка заданий печати, которые поставлены в очередь для обработки с помощью printerShare. |
| [Создание задания](../api/printershare-post-jobs.md) | [Printjob](printjob.md) | Создайте задание печати для printerShare. Чтобы начать печать задания, используйте команду [start](../api/printjob-start.md). |
| [Список allowedUsers](../api/printershare-list-allowedusers.md) | Коллекция объектов [user](user.md) | Получение списка пользователей, которым предоставлен доступ для отправки заданий печати в связанную общую папку принтера. |
| [Добавление allowedUser](../api/printershare-post-allowedusers.md) | Нет | Предоставьте указанному пользователю доступ для отправки заданий печати в связанную общую папку принтера. |
| [Удаление allowedUser](../api/printershare-delete-alloweduser.md) | Нет | Отмените доступ к общей папке принтера у указанного пользователя. |
| [Список allowedGroups](../api/printershare-list-allowedgroups.md) | Коллекция [group](group.md) | Получение списка групп, которым предоставлен доступ для отправки заданий печати в связанную общую папку принтера. |
| [Добавление allowedGroup](../api/printershare-post-allowedgroups.md) | Нет | Предоставьте указанной группе доступ для отправки заданий печати в связанную общую папку принтера. |
| [Удаление allowedGroup](../api/printershare-delete-allowedgroup.md) | Нет | Отмените доступ к общей папке принтера из указанной группы. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Идентификатор printerShare. Только для чтения.|
|displayName|Строка|Имя общей папки принтера, которую должны отобразить клиенты печати.|
|createdDateTime|DateTimeOffset|DateTimeOffset при создании общей папки принтера. Только для чтения.|
|manufacturer|String|Производитель, указанный принтером, связанным с этой общей папкой принтера. Только для чтения.|
|model|String|Имя модели, сообщаемое принтером, связанным с этой общей папкой принтера. Только для чтения.|
|isAcceptingJobs|Логическое|Принимает ли принтер, связанный с этой общей папкой принтера, новые задания печати.|
|defaults|[printerDefaults](printerdefaults.md)|Параметры печати принтера по умолчанию, связанного с этой общей папкой принтера.|
|capabilities|[printerCapabilities](printercapabilities.md)|Возможности принтера, связанного с этой общей папкой принтера.|
|расположение;|[printerLocation](printerlocation.md)|Физическое и (или) организационное расположение принтера, связанного с этой общей папкой принтера.|
|status|[printerStatus](printerstatus.md)|Состояние обработки принтера, связанного с этой общей папкой принтера, включая все ошибки. Только для чтения.|
|allowAllUsers|Логическое|Если значение равно true, всем пользователям и группам будет предоставлен доступ к этой общей папке принтера. Это заменяет списки разрешений, определенные свойствами навигации **allowedUsers** и **allowedGroups** .|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Принтера|[printer](printer.md)|Принтер, с котором связан этот общий принтер. |
|allowedUsers|Коллекция объектов [user](user.md)|Пользователи, у которых есть доступ к печати с помощью принтера.|
|allowedGroups|[group](group.md)|Группы, пользователи которых имеют доступ к печати с помощью принтера.|
|jobs|[Коллекция printJob](printjob.md)| Список заданий, которые поставлены в очередь для печати принтером, связанным с этой общей папкой принтера.|

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


