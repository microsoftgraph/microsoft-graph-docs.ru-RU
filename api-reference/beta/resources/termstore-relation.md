---
title: Тип ресурса связи
description: Представляет связь между терминами в банке терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2e8f4dc8b82c496909f5b150829d9fb4e114ba59
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973591"
---
# <a name="relation-resource-type"></a>Тип ресурса связи

Пространство имен: Microsoft. Graph. банка

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет связь между [терминами](../resources/termstore-term.md) в [банке]терминов. В настоящее время поддерживаются два типа отношений: ПИН-код и повторное использование. 

В контактном отношении термин может быть закреплен под другим термином в другом наборе терминов. В закрепленной связи новые дочерние элементы для термина можно добавить только в набор терминов, в котором был создан термин. Любое изменение в иерархии под термином отражается на тех наборах, в которых термин был закреплен. 

Отношение повторного использования аналогично закрепленному отношению, за исключением того, что изменения повторно используемого термина можно выполнить из любой иерархии, в которой этот термин используется повторно. Кроме того, изменение иерархии, выполненное для повторно используемого термина, не отражается в других наборах терминов, в которых термин используется повторно.

Наследуется от [объекта Entity](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список отношений](../api/termstore-term-list-relations.md)|Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)|Получение списка объектов **relation** .|
|[Создание отношения](../api/termstore-relation-post.md)|[Microsoft. Graph. Банк. отношение](../resources/termstore-relation.md)|Создание объекта **связи** .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор отношения.|
|Отношение|String|Тип отношения. Возможные значения: `pin`, `reuse`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|фромтерм|[Microsoft. Graph. Банк. Term](../resources/termstore-term.md)|[Термин] "от" отношения. Термин, в котором определено отношение. Значение NULL указывает на то, что отношение напрямую с [набором]. |
|set|[Microsoft. Graph. банка. Set](../resources/termstore-set.md)|[Набор] , в котором соотношение является релевантным.|
|тотерм|[Microsoft. Graph. Банк. Term](../resources/termstore-term.md)|[Термин] "Кому" отношения. Термин, для которого определен реалтионшип.|

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
[банком]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "TermRelation is the entity for mapping relations between different terms",
  "keywords": "termRelation,facet,resource",
  "section": "documentation",
  "tocPath": "TermRelation",
  "tocBookmarks": {
    "Resources/termStore.relation": "#"
  },
  "suppressions": []
}
-->


