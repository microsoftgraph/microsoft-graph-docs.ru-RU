---
title: тип ресурса связи
description: Представляет связь между терминами в магазине терминов.
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 88276a66949a55f0ee953f556977a2380ed415d9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128034"
---
# <a name="relation-resource-type"></a>тип ресурса связи

Пространство имен: microsoft.graph.termStore

Представляет связь между [терминами в](../resources/termstore-term.md) магазине [терминов.] В настоящее время поддерживаются два типа отношений: **пин-код** **и повторное использование.** 

В связи с пин-кодом термин можно закрепить под другим термином в другом наборе терминов. В закрепленных отношениях новые дети могут быть добавлены к термину только в наборе терминов, в которых был создан термин. Любое изменение иерархии в термине отражается в наборах, в которых был закреплен термин. 

Отношение повторного использования аналогично закрепленным отношениям, за исключением того, что изменения в термине повторного использования могут быть сделаны из любой иерархии, в которой термин повторно. Кроме того, изменение иерархии повторного термина не отражается в других наборах терминов, в которых термин повторно.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Отношения списка](../api/termstore-term-list-relations.md)|[коллекция microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Извлечение списка **объектов связи.**|
|[Создание связи](../api/termstore-relation-post.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Создайте новый **объект связи.**|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID связи.|
|Отношение|microsoft.graph.termStore.relationType|Тип связи. Возможные значения: `pin`, `reuse`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|fromTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Срок [отношения.] Термин, от которого определяются отношения. *Null* value would indicate the relation is directly with the [set.] |
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|[Набор,] в котором отношение имеет значение.|
|toTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Срок [отношения.] Термин, к которому определяется отношение.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.relation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "String (identifier)",
  "relationship": "String"
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.relations]: termstore-relation.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[store]: ../resources/termstore-store.md
[термин]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "TermRelation is the entity for mapping relations between different terms",
  "keywords": "termRelation,facet,resource",
  "section": "documentation",
  "tocPath": "TermRelation",
  "tocBookmarks": {
    "Resources/termStore.relation&quot;: &quot;#"
  },
  "suppressions": []
}
-->


