---
title: тип ресурсов externalGroup
description: Представляет внешнюю группу, используемую для набора разрешений на externalItems, добавленных в подключение Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3f0c6adbd47d1823b82e19d3fb9a352e26391da9
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467827"
---
# <a name="externalgroup-resource-type"></a>тип ресурсов externalGroup

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет внешнюю группу. Внешние группы (наряду Azure Active Directory пользователями и группами) используются для набора разрешений **на externalItems,** добавленных в подключение Microsoft Graph. Используйте **externalGroups** для представления Azure Active Directory групп или групп-подобных конструкций (например, бизнес-подразделений, Teams и son on), которые определяют разрешение на контент в внешнем источнике данных.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание externalGroup](../api/externalconnectors-externalconnection-post-groups.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Создайте новый **объект externalGroup.**|
|[Удаление externalGroup](../api/externalconnectors-externalgroup-delete.md)|Нет|Удаление **объекта externalGroup.**|
|[Создание участников](../api/externalconnectors-externalgroup-post-members.md)|[microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md)|Создание нового **внешнего объектаGroupMember.**|

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | Уникальный ID внешней группы в подключении. Он должен быть альфа-числом и может иметь длину до 128 символов. |
| displayName | String | Дружеское имя внешней группы. Необязательное.                                                                       |
| description | String | Описание внешней группы. Необязательное.                                                                         

## <a name="relationships"></a>Связи

| Связь | Тип                                                                  | Описание                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| members      | [коллекция microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md) | Член, добавленный в **externalGroup.** В качестве участников можно Azure Active Directory пользователей, Azure Active Directory групп или других **внешних групп.** |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
