---
title: тип ресурсов externalGroup
description: Представляет группу, не Azure Active Directory.
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2f944032cbe58972ecab1075ca01053817f9de63
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697551"
---
# <a name="externalgroup-resource-type"></a>тип ресурсов externalGroup

Пространство имен: microsoft.graph.externalConnectors

Представляет группу, не Azure Active Directory.

Внешние группы определяют разрешения на контент в внешнем источнике данных. Эти внешние группы можно использовать в записях [на acl](../resources/externalconnectors-externalitem.md) [externalItem](../resources/externalconnectors-externalitem.md).

Примерами внешних групп являются бизнес-подразделения и группы работы.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание externalGroup](../api/externalconnectors-externalconnection-post-groups.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Создайте новый **объект externalGroup.**|
|[Get externalGroup](../api/externalconnectors-externalgroup-get.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Получите **объект externalGroup.**|
|[Обновление externalGroup](../api/externalconnectors-externalgroup-update.md)|[microsoft.graph.externalConnectors.externalGroup](../resources/externalconnectors-externalgroup.md)|Обновление свойств объекта **externalGroup.**|
|[Удаление externalGroup](../api/externalconnectors-externalgroup-delete.md)|Нет|Удаление **объекта externalGroup.**|

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | Уникальный ID внешней группы в подключении. Он должен быть альфа-числом и может иметь длину до 128 символов. |
| displayName | String | Дружеское имя внешней группы. Необязательный параметр.                                                                       |
| description | String | Описание внешней группы. Необязательный параметр.        

## <a name="relationships"></a>Связи

| Связь | Тип                                                                  | Описание                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| members      | [коллекция microsoft.graph.externalConnectors.identity](../resources/externalconnectors-identity.md) | Член, добавленный в **externalGroup.** Вы можете добавить Azure Active Directory, Azure Active Directory групп или **externalGroup** в качестве участников. |

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup",
  "baseType": "microsoft.graph.entity",
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
