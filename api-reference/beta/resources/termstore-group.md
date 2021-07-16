---
author: mohitpcad
title: Тип группового ресурса
doc_type: resourcePageType
description: Представляет группу, используемую в магазине терминов.
localization_priority: Normal
ms.prod: taxonomy
ms.openlocfilehash: ec2e9609b2de278d2596d42b18cae2fe450efd86
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456361"
---
# <a name="group-resource-type"></a>Тип группового ресурса

Пространство имен: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Представляет группу, используемую в магазине [терминов.](../resources/termstore-store.md) Группа — это логическая иерархия, которая содержит коллекцию наборов под ней. 

Наследует от [объекта](../resources/entity.md).


## <a name="methods"></a>Методы

| Метод                                                   | Тип возвращаемых данных       |    Описание
|:---------------------------------------------------------|:------------------|:---------------------
| [Создание группы](../api/termstore-group-post.md)                     | [microsoft.graph.termStore.group] | Создание группы в магазине [терминов.]
| [Получение группы](../api/termstore-group-get.md)                           | [microsoft.graph.termStore.group] | Извлечение данных группы в магазине [терминов.]
| [Удаление группы](../api/termstore-group-delete.md)                     | Нет |  Удаление группы в магазине [терминов].

## <a name="properties"></a>Свойства

| Свойство             | Тип               | Описание
|:---------------------|:-------------------|:------------------------------------
| createdDateTime      | DateTimeOffset     | Дата и время создания группы. Только для чтения.
| description          | string             | Описание с подробными сведениями об использовании термина.
| id                   | string             | Уникальный идентификатор группы. Только для чтения.
| displayName          | string             | Имя группы.
| scope                | string              | Возвращает тип группы. Возможные значения : "глобальный", "системный" и "siteCollection".
| parentSiteId         | String             | Id родительского сайта этой группы.

## <a name="relationships"></a>Связи
| Связь       | Тип                        | Описание
|:-------------------|:----------------------------|:--------------------------
| наборы           | [коллекция microsoft.graph.termStore.set][] | Все наборы в группе в магазине [терминов].

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON **группового** ресурса.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.group",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.termStore.group",
  "id": "string",
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "scope" : "microsoft.graph.termStore.groupScope",
  "displayName": "string",
  "parentSiteId" : "string"
}
```



[identitySet]: identitySet.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[магазин]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
<!--
{
  "type": "#page.annotation",
  "description": "TermGroup is the entity used for managing permissions for the termSets in termStore",
  "keywords": "termGroup,facet,resource",
  "section": "documentation",
  "tocPath": "TermGroup",
  "tocBookmarks": {
    "Resources/termStore.group&quot;: &quot;#"
  },
  "suppressions": []
}
-->


