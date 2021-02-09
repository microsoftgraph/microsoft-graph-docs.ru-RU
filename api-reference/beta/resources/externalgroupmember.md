---
title: Тип ресурса externalGroupMember
description: Представляет члена внешней группы, используемой для изменения разрешений для внешнего контента, добавленного в Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1e86fb275b941b7a3033999fedd4c71aa3ac1de1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161693"
---
# <a name="externalgroupmember-resource-type"></a>Тип ресурса externalGroupMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет члена внешней группы, [используемой для](externalgroup.md) изменения разрешений для внешнего контента, добавленного в Microsoft Graph.

## <a name="methods"></a>Методы

| Метод                                                              | Тип возвращаемых данных         | Описание                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [Создание externalGroupMember](../api/externalgroup-post-members.md) | externalGroupMember | Создание объекта **externalGroupMember.** |
| [Удаление externalGroupMember](../api/externalgroupmember-delete.md)  | Нет                | Удаление объекта **externalGroupMember.**   |

## <a name="properties"></a>Свойства

| Свойство       | Тип                    | Описание                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | Уникальный ИД участника. Это будет objectId в случае пользователей или групп Azure Active Directory и свойство **id** **внешней группы** в случае внешних групп.                                    |
| type           | externalGroupMemberType | Тип участника, добавленного во внешнюю группу. Возможные значения: `user` или когда идентификатор `group` **identitySource** и только `azureActiveDirectory` `group` тогда, когда идентификатор **identitySource** имеет значение `external` . |
| identitySource | identitySourceType      | Источник удостоверений, к которой принадлежит участник. Возможные значения: `azureActiveDirectory`, `external`.                                                                                         |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
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
