---
title: Тип ресурса Екстерналграуп
description: Представляет внешнюю группу, используемую для установки разрешений для Екстерналитемс, добавленных в подключение Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c258df9e6f20cf7a19e291fd298ad66345a72949
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193939"
---
# <a name="externalgroup-resource-type"></a>Тип ресурса Екстерналграуп

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет внешнюю группу. Внешние группы (наряду с пользователями и группами Azure Active Directory) используются для установки разрешений **екстерналитемс** , добавляемых в подключение Microsoft Graph. Используйте **екстерналграупс** для представления групп, не относящихся к Azure Active Directory, или конструкций, подобных группам (таких как бизнес-единицы, Teams и налево), которые определяют разрешения на доступ к контенту во внешнем источнике данных.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание Екстерналграуп](../api/externalconnection-post-groups.md)|[екстерналграуп](../resources/externalgroup.md)|Создание нового объекта **екстерналграуп** .|
|[Удаление Екстерналграуп](../api/externalgroup-delete.md)|Нет|Удаление объекта **екстерналграуп** .|
|[Создание участников](../api/externalgroup-post-members.md)|[екстерналграупмембер](../resources/externalgroupmember.md)|Создание нового объекта **екстерналграупмембер** .|

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | String | Уникальный идентификатор внешней группы в подключении. Он должен состоять из буквенно-цифровых символов и иметь длину до 128 символов. |
| displayName | String | Понятное имя внешней группы. Необязательно.                                                                       |
| description | String | Описание внешней группы. Необязательно.                                                                         

## <a name="relationships"></a>Связи

| Связь | Тип                                                                  | Описание                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| members      | Коллекция [екстерналграупмембер](../resources/externalgroupmember.md) | Член, добавленный в объект **екстерналграуп**. Вы можете добавлять пользователей Azure Active Directory, группы Azure Active Directory или другие **екстерналграупс** в качестве участников. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "baseType": "",
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
