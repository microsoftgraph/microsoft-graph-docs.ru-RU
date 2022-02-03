---
author: vishriv
title: Тип группового ресурса
doc_type: resourcePageType
description: Представляет группу, используемую в магазине терминов.
ms.localizationpriority: medium
ms.prod: taxonomy
ms.openlocfilehash: 1fa25c258050f1bf5cf2cea3e95a13e95f9b8125
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339916"
---
# <a name="group-resource-type"></a>Тип группового ресурса

Пространство имен: microsoft.graph.termStore


Представляет группу, используемую в магазине [терминов](../resources/termstore-store.md). Группа — это логическая иерархия, которая содержит коллекцию наборов под ней. 

Наследуется [от сущности](../resources/entity.md).


## <a name="methods"></a>Методы

| Метод                                                   | Тип возвращаемых данных       |    Описание      |
|:---------------------------------------------------------|:------------------|:---------------------
| [Создание группы](../api/termstore-group-post.md)                     | [microsoft.graph.termStore.group] | Создание группы в магазине [терминов]. |
| [Получение группы](../api/termstore-group-get.md)                           | [microsoft.graph.termStore.group] | Извлечение данных группы в магазине [терминов]. |
| [Удаление группы](../api/termstore-group-delete.md)                     | Нет |  Удаление группы в магазине [терминов]. |

## <a name="properties"></a>Свойства

| Свойство             | Тип               | Описание                        |
|:---------------------|:-------------------|:------------------------------------
| createdDateTime      | DateTimeOffset     | Дата и время создания группы. Только для чтения. |
| description          | string             | Описание, которое дает сведения об использовании термина. |
| id                   | string             | Уникальный идентификатор группы. Только для чтения. |
| displayName          | string             | Имя группы. |
| scope                | string              | Возвращает тип группы. Возможные значения: `global`, `system` и `siteCollection`. |
| parentSiteId         | string             | ID родительского сайта этой группы. |

## <a name="relationships"></a>Связи
| Связь       | Тип                        | Описание              |
|:-------------------|:----------------------------|:--------------------------
| наборы           | [коллекция microsoft.graph.termStore.set][] | Все наборы в группе в магазине [терминов]. |

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


