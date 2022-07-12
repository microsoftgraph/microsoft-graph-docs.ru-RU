---
title: Тип ресурса relation
description: Представляет связь между терминами в хранилище терминов.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 18753cf6cb246eea25f9a497ebebc197ac23cb93
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732662"
---
# <a name="relation-resource-type"></a>Тип ресурса relation

Пространство имен: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет связь между [терминами](../resources/termstore-term.md) в хранилище [терминов]. В настоящее время поддерживаются два типа связей: закрепление и повторное использование. 

В связи с закреплением термин можно закрепить под другим термином в другом наборе терминов. В закрепленной связи новые дочерние элементы термина можно добавить только в набор терминов, в котором был создан термин. Любое изменение иерархии в термине отражается в наборах, в которых был закреплен термин. 

Отношение повторного использования аналогично закрепленной связи, за исключением того, что изменения в повторно используемом термине могут быть внесены из любой иерархии, в которой термин используется повторно. Кроме того, изменение иерархии, внесенное в повторно используемый термин, не отражается в других наборах терминов, в которых термин используется повторно.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление связей](../api/termstore-term-list-relations.md)|[Коллекция microsoft.graph.termstore.relation](../resources/termstore-relation.md)|Получение списка объектов **отношения** .|
|[Создание отношения](../api/termstore-relation-post.md)|[microsoft.graph.termstore.relation](../resources/termstore-relation.md)|Создайте объект **отношения** .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор отношения.|
|Отношение|String|Тип отношения. Возможные значения: `pin`, `reuse`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|fromTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|От [термина отношения] . Термин, из которого определена связь. Значение NULL указывает, что отношение непосредственно с [набором]. |
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Набор [,] в котором отношение релевантно.|
|toTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Термин [отношения.] Термин, с которым определена связь.|

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
[Термин]: ../resources/termstore-term.md
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


