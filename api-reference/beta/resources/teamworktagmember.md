---
title: тип ресурса teamworkTagMember
description: Представляет пользователя в команде с тегом, примененным к ним.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 73666dd19720e6d8882bb16fd90c612097e41d10
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059885"
---
# <a name="teamworktagmember-resource-type"></a>тип ресурса teamworkTagMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя в команде, к которой применяется тег.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список командной работыTagMembers](../api/teamworktagmember-list.md)|**коллекция teamworkTagMember**|Получите список участников стандартного тега в команде и их свойства.|
|[Получить командную работуTagMember](../api/teamworktagmember-get.md)|**teamworkTagMember**|Получите свойства и отношения участника стандартного тега в команде.|
|[Удаление командной работыTagMember](../api/teamworktagmember-delete.md)|Нет.|Удаление участника из стандартного тега в команде.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя отображения участника.|
|ID|Строка|ID участника.|
|tenantID|Строка|ID клиента, в который входит член тега.|
|userID|Строка|Пользовательский ID участника.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "ID",
  "@odata.type": "microsoft.graph.teamworkTagMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagMember",
  "ID": "String (Identifier)",
  "displayName": "String",
  "tenantID": "String",
  "userID": "String"
}
```

