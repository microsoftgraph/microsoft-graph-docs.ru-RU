---
title: тип ресурса teamworkTagMember
description: Представляет пользователя в команде с тегом, примененным к ним.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: b8e6d70a8249168383f2bc1b0e6d8884525855ec
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534518"
---
# <a name="teamworktagmember-resource-type"></a>тип ресурса teamworkTagMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя в команде, к которой применяется тег.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список командной работыTagMembers](../api/teamworktagmember-list.md)|[**коллекция teamworkTagMember**](teamworktagmember.md)|Получите список участников стандартного тега в команде и их свойства.|
|[Создание командной работыTagMember](../api/teamworktagmember-post.md)|[**teamworkTagMember**](teamworktagmember.md)|Создайте новый **объект teamworkTagMember.**|
|[Получить командную работуTagMember](../api/teamworktagmember-get.md)|[**teamworkTagMember**](teamworktagmember.md)|Получите свойства и отношения участника стандартного тега в команде.|
|[Удаление командной работыTagMember](../api/teamworktagmember-delete.md)|Нет|Удаление участника из стандартного тега в команде.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя отображения участника.|
|Идентификатор|Строка|ID участника.|
|tenantID|Строка|ID клиента, в который входит член тега.|
|userID|Строка|Пользовательский ID участника.|

## <a name="relationships"></a>Отношения
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

