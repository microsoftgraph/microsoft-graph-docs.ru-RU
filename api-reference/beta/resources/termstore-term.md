---
title: Тип ресурса term
description: Определяет сущность термина в хранилище терминов.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 0207c740d52f7e7401ed6c741cf8d9134ec47eb1
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730282"
---
# <a name="term-resource-type"></a>Тип ресурса term

Пространство имен: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет термин, используемый в банках [терминов]. Термин можно использовать для представления объекта, который затем можно использовать в качестве метаданных для пометки содержимого. Несколько терминов можно упорядочить в наборе иерархическим [образом].

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список дочерних элементов](../api/termstore-term-list-children.md)|[Коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)|Получение дочерних элементов первого уровня термина в хранилище [терминов].|
|[Перечисление связей](../api/termstore-term-list-relations.md)|[Коллекция microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Получение связей термина в хранилище [терминов].|
|[Создание отношения](../api/termstore-relation-post.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Создайте новое отношение для термина или [набора в] хранилище [терминов].|
|[Создание термина](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Создайте объект термина в хранилище [терминов].|
|[Получение термина](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Чтение свойств и связей объекта термина в хранилище  [терминов].|
|[Срок обновления](../api/termstore-term-update.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Обновление свойств объекта термина в хранилище [терминов].|
|[Удалить термин](../api/termstore-term-delete.md)|Нет|Удаление объекта термина в хранилище [терминов].|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания термина. Только для чтения.|
|Описания|[Коллекция microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md)|Описание термина, который зависит от languageTag.|
|id|String|Уникальный идентификатор термина. Только для чтения.|
|Метки|[Коллекция microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md)|Метка метаданных для термина.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения термина. Только для чтения.|
|properties|[Коллекция microsoft.graph.keyValue](../resources/keyvalue.md)|Коллекция свойств термина.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|children|[Коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)|Дочерние элементы текущего термина.|
|Отношения|[Коллекция microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Чтобы указать, какие термины связаны с текущим термином как закрепленные или повторно используемые.|
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Набор [,] в котором создается термин.|

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


