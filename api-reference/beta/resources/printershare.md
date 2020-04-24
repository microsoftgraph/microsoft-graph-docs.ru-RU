---
title: Тип ресурса Принтершаре
description: Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8aa9312bf8b7e8f9a2cec049b8275d4ce7a04012
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806844"
---
# <a name="printershare-resource-type"></a>Тип ресурса Принтершаре

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List](../api/print-list-printershares.md) | Коллекция [принтершаре](printershare.md) | Получение списка общих принтеров в клиенте. |
| [получение](../api/printershare-get.md); | [принтершаре](printershare.md) | Чтение свойств и связей объекта **принтершаре** . |
| [Обновление](../api/printershare-update.md) | [принтершаре](printershare.md) | Обновление объекта **принтершаре** . |
| [удаление](../api/printershare-delete.md); | Нет | Отменяет общий доступ к принтеру. |
| [Список allowedUsers](../api/printershare-list-allowedusers.md) | Коллекция [userIdentity](useridentity.md) | Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный общий принтер. |
| [Добавление allowedUser](../api/printershare-post-allowedusers.md) | Нет | Предоставьте заданному пользователю доступ на отправку заданий печати в соответствующую общую папку принтера. |
| [Удаление allowedUser](../api/printershare-delete-alloweduser.md) | Нет | Отозвать доступ к общему принтеру для указанного пользователя. |
| [Список allowedGroups](../api/printershare-list-allowedgroups.md) | Коллекция [удостоверений](identity.md) | Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный общий принтер. |
| [Добавление allowedGroup](../api/printershare-post-allowedgroups.md) | Нет | Предоставление указанному групповому доступу на отправку заданий печати на связанный общий принтер. |
| [Удаление allowedGroup](../api/printershare-delete-allowedgroup.md) | Нет | Отзыв доступа к общему принтеру из указанной группы. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Идентификатор Принтершаре. Только для чтения.|
|name|String|Имя общего принтера, который должен отображаться клиентами печати.|
|createdDateTime|DateTimeOffset|Значение DateTimeOffset при создании общего ресурса принтера. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Printer|[Printer](printer.md)|Принтер, с которым связан этот общий принтер. |
|алловедусерс|Коллекция [userIdentity](useridentity.md)|Пользователи, у которых есть доступ к печати с помощью принтера.|
|алловедграупс|[identity](identity.md)|Группы, у которых пользователи имеют доступ к печати с помощью принтера.|

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
  "name": "String",
  "createdDateTime": "String (timestamp)"
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
