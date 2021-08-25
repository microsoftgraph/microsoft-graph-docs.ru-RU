---
title: тип ресурса терминов
description: Определяет сущность терминов в магазине терминов.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 5a8c429a20ed533c6de8fb11bb13aa877e2c41be
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514980"
---
# <a name="term-resource-type"></a>тип ресурса терминов

Пространство имен: microsoft.graph.termStore

Представляет термин, используемый в магазине [терминов.] Термин можно использовать для представления объекта, который затем можно использовать в качестве метаданных для тегов контента. Несколько терминов могут быть организованы иерархическим образом в [наборе].

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список дочерних элементов](../api/termstore-term-list-children.md)|[коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)|Получите детей первого уровня термина в магазине [терминов.]|
|[Отношения списка](../api/termstore-term-list-relations.md)|[коллекция microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Получите отношения термина в магазине [терминов.]|
|[Создание связи](../api/termstore-relation-post.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Создание нового отношения для термина или набора [в] магазине [терминов.]|
|[Создание термина](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Создание нового объекта терминов в магазине [терминов.]|
|[Получить термин](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Ознакомьтесь с свойствами и отношениями объекта терминов в магазине [терминов.]|
|[Термин Update](../api/termstore-term-update.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Обновление свойств объекта терминов в магазине [терминов.]|
|[Удаление термина](../api/termstore-term-delete.md)|Нет.|Удаление объекта терминов в магазине [терминов.]|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания терминов. Только для чтения.|
|описания|[коллекция microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md)|Описание термина, который зависит от languageTag.|
|id|Строка|Уникальный идентификатор термина. Только для чтения.|
|метки|[коллекция microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md)|Метки метаданных для термина.|
|lastModifiedDateTime|DateTimeOffset|Последняя дата и время изменения срока. Только для чтения.|
|properties|[коллекция microsoft.graph.keyValue](../resources/keyvalue.md)|Коллекция свойств в термине.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|children|[коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)|Дети текущего срока.|
|отношения|[коллекция microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Чтобы указать, какие термины связаны с текущим термином как закрепленные или повторно.|
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|[Набор,] в котором создается термин.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.term",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.term",
  "id": "String (identifier)",
  "labels": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedLabel"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "descriptions": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedDescription"
    }
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ]
}
```

[магазин]: ../resources/termstore-store.md
[set]: ../resources/termstore-set.md
[term]: ../resources/termstore-term.md
[group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Term is the entity used for tagging in termStore",
  "keywords": "term,facet,resource",
  "section": "documentation",
  "tocPath": "Terms",
  "tocBookmarks": {
    "Resources/termstore-term&quot;: &quot;#"
  },
  "suppressions": []
}
-->


