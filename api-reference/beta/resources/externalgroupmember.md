---
title: Тип ресурса Екстерналграупмембер
description: Представляет члена объекта Екстерналграуп, используемого для установки разрешений на доступ к внешнему контенту, добавленному в Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 19b5c5094501215cc3ffd3e852ba6ca427807988
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193936"
---
# <a name="externalgroupmember-resource-type"></a>Тип ресурса Екстерналграупмембер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет члена объекта [екстерналграуп](externalgroup.md) , используемого для установки разрешений на доступ к внешнему контенту, добавленному в Microsoft Graph.

## <a name="methods"></a>Методы

| Метод                                                              | Тип возвращаемых данных         | Описание                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [Создание Екстерналграупмембер](../api/externalgroup-post-members.md) | екстерналграупмембер | Создание нового объекта **екстерналграупмембер** . |
| [Удаление Екстерналграупмембер](../api/externalgroupmember-delete.md)  | Нет                | Удаление объекта **екстерналграупмембер** .   |

## <a name="properties"></a>Свойства

| Свойство       | Тип                    | Описание                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | Уникальный идентификатор элемента. Это идентификатор objectId в случае с пользователями или группами Azure Active Directory, а также свойством **ID** **екстерналграуп** в случае внешних групп.                                    |
| type           | екстерналграупмембертипе | Тип элемента, добавляемого во внешнюю группу. Возможные значения: `user` или `group` , если **идентитисаурце** , `azureActiveDirectory` и только в том `group` случае, если **идентитисаурце** `external` . |
| идентитисаурце | идентитисаурцетипе      | Источник удостоверения, к которому принадлежит член. Возможные значения: `azureActiveDirectory`, `external`.                                                                                         |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
