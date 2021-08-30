---
title: тип ресурсов externalGroup
description: Представляет группу, не Azure Active Directory.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5fbfcb8b462b490b33519f04268c505871613a24
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697389"
---
# <a name="externalgroup-resource-type"></a>тип ресурсов externalGroup

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пространство имен: microsoft.graph.externalConnectors

Представляет группу, не Azure Active Directory.

Внешние группы определяют разрешения на контент в внешнем источнике данных. Эти внешние группы можно использовать в записях [на acl](../resources/externalconnectors-externalitem.md) [externalItem](../resources/externalconnectors-externalitem.md).

Примерами внешних групп являются бизнес-подразделения и группы работы.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание externalGroup](../api/externalconnectors-externalconnection-post-groups.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Создайте новый **объект externalGroup.**|
|[Удаление externalGroup](../api/externalconnectors-externalgroup-delete.md)|Нет|Удаление **объекта externalGroup.**|
|[Создание члена](../api/externalconnectors-externalgroup-post-members.md)|[microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md)|Создание нового **внешнего объектаGroupMember.**|

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | Строка | Уникальный ID внешней группы в подключении. Он должен быть альфа-числом и может иметь длину до 128 символов. |
| displayName | Строка | Дружеское имя внешней группы. Необязательный параметр.                                                                       |
| description | Строка | Описание внешней группы. Необязательный параметр.                                                                         

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
