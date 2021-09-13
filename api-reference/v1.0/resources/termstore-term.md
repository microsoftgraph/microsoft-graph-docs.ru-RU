---
title: тип ресурса терминов
description: Определяет сущность терминов в магазине терминов.
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 570a4a365b86a48859608798ba3eb5be9958cd1e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084036"
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
|[Удаление термина](../api/termstore-term-delete.md)|Нет|Удаление объекта терминов в магазине [терминов.]|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания терминов. Только для чтения.|
|описания|[коллекция microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md)|Описание термина, который зависит от languageTag.|
|id|String|Уникальный идентификатор термина. Только для чтения.|
|метки|[коллекция microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md)|Метки метаданных для термина.|
|lastModifiedDateTime|DateTimeOffset|Последняя дата и время изменения срока. Только для чтения.|
|properties|[коллекция microsoft.graph.keyValue](../resources/keyvalue.md)|Коллекция свойств в термине.|

## <a name="relationships"></a>Отношения
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

[store]: ../resources/termstore-store.md
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


