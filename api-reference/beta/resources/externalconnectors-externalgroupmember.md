---
title: тип ресурса externalGroupMember
description: Представляет члена externalGroup, используемого для набора разрешений на внешний контент, добавленный в Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e3626c718360982bf79cb9757a13e4b4c01669cd
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467823"
---
# <a name="externalgroupmember-resource-type"></a>тип ресурса externalGroupMember

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет члена внешней [](externalconnectors-externalgroup.md) группы, используемой для набора разрешений на внешний контент, добавленный в Microsoft Graph.

## <a name="methods"></a>Методы

| Метод                                                              | Тип возвращаемых данных         | Описание                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [Создание externalGroupMember](../api/externalconnectors-externalgroup-post-members.md) | [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) | Создание нового **внешнего объектаGroupMember.** |
| [Удаление externalGroupMember](../api/externalconnectors-externalgroupmember-delete.md)  | Нет                | Удаление **внешнего объектаGroupMember.**   |

## <a name="properties"></a>Свойства

| Свойство       | Тип                    | Описание                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | Уникальный ID участника. Это будет objectId в случае Azure Active Directory пользователей или групп и **id** свойства **externalGroup** в случае внешних групп.                                    |
| type           | microsoft.graph.externalConnectors.externalGroupMemberType | Тип участника, добавленного во внешнюю группу. Возможные значения: или когда identitySource является и только `user` `group`  `azureActiveDirectory` `group` тогда, когда **identitySource** `external` является . |
| identitySource | microsoft.graph.externalConnectors.identitySourceType      | Источник удостоверений, к которой принадлежит член. Возможные значения: `azureActiveDirectory`, `external`.                                                                                         |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
