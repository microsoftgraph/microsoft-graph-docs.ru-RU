---
title: Тип ресурса externalGroup
description: Представляет внешнюю группу, используемую для изменения разрешений для externalItems, добавленных к подключению Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2e9d8e3a605f1c3df39b13607f82e7541d59e62e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161714"
---
# <a name="externalgroup-resource-type"></a>Тип ресурса externalGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет внешнюю группу. Внешние группы (наряду с пользователями и группами Azure Active Directory) используются для изменения разрешений **для externalItems,** добавленных к подключению Microsoft Graph. Используйте **externalGroups** для представления групп, не в том числе Azure Active Directory, или конструкций, похожих на группы (таких как бизнес-единицы, Teams и другие), которые определяют разрешения на содержимое во внешнем источнике данных.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание externalGroup](../api/externalconnection-post-groups.md)|[externalGroup](../resources/externalgroup.md)|Создание объекта **externalGroup.**|
|[Удаление externalGroup](../api/externalgroup-delete.md)|Нет|Удаление объекта **externalGroup.**|
|[Создание участников](../api/externalgroup-post-members.md)|[externalGroupMember](../resources/externalgroupmember.md)|Создание объекта **externalGroupMember.**|

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | Уникальный ИД внешней группы в соединении. Она должна быть букво-цифрой и длиной до 128 символов. |
| displayName | String | Имя внешней группы. Необязательный параметр.                                                                       |
| description | String | Описание внешней группы. Необязательный параметр.                                                                         

## <a name="relationships"></a>Связи

| Связь | Тип                                                                  | Описание                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| members      | [Коллекция externalGroupMember](../resources/externalgroupmember.md) | Член, добавленный в **внешнюю группу.** В качестве участников можно добавить пользователей Azure Active Directory, группы Azure Active Directory или другие **внешние группы.** |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
