---
title: Тип ресурса термина
description: Определяет сущность термина в банке терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 831a873d245424bcb92c7281b1bbdc97b29223bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075562"
---
# <a name="term-resource-type"></a>Тип ресурса термина

Пространство имен: Microsoft. Graph. банка

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет термин, используемый в [банке]терминов. Термин можно использовать для представления объекта, который затем можно использовать в качестве метаданных для тега конент. Несколько терминов можно организовать иерархически в пределах [набора].

Наследуется от [объекта Entity](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список дочерних элементов](../api/termstore-term-list-children.md)|Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)|Получение потомков первого уровня термина в [банке]терминов.|
|[Список отношений](../api/termstore-term-list-relations.md)|Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)|Получение отношений терминов в [банке]терминов.|
|[Создание отношения](../api/termstore-relation-post.md)|[Microsoft. Graph. Банк. отношение](../resources/termstore-relation.md)|Создание нового отношения для термина или [набора] в [банке]терминов.|
|[Создание термина](../api/termstore-term-post.md)|[Microsoft. Graph. Банк. Term](../resources/termstore-term.md)|Создайте новый объект Term в [банке]терминов.|
|[Получение термина](../api/termstore-term-get.md)|[Microsoft. Graph. Банк. Term](../resources/termstore-term.md)|Чтение свойств и связей объекта Term в  [банке]терминов.|
|[Обновление термина](../api/termstore-term-update.md)|[Microsoft. Graph. Банк. Term](../resources/termstore-term.md)|Обновление свойств объекта Term в [банке]терминов.|
|[Удаление термина](../api/termstore-term-delete.md)|Нет|Удаление объекта Term в [банке]терминов.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания терминов. Только для чтения|
|состояний|Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализеддескриптион](../resources/termstore-localizeddescription.md)|Описание термина, зависящего от Лангуажетаг|
|id|String|Уникальный идентификатор термина. Только чтение|
|Метка|Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализедлабел](../resources/termstore-localizedlabel.md)||Метаданные метки для термина|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения термина. Только для чтения|
|properties|Коллекция [Microsoft. Graph. ключзначение](../resources/keyvalue.md)|Коллекция свойств термина|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|children|Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)|Дочерние элементы текущего термина|
|отношениях|Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)|Указание терминов, связанных с текущим термином, в качестве закрепления или повторного использования|
|set|[Microsoft. Graph. банка. Set](../resources/termstore-set.md)|[Набор] , в котором создается термин|

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
    "Resources/termstore-term": "#"
  },
  "suppressions": []
}
-->


