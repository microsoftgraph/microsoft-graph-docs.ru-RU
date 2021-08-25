---
title: набор типа ресурса
description: Представляет набор в магазине терминов.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: d56bc436dca1c645d7e5d24face75a9bf5acd957
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514986"
---
# <a name="set-resource-type"></a>набор типа ресурса

Пространство имен: microsoft.graph.termStore

Представляет набор, используемый в магазине [терминов.] Набор представляет собой блок, содержащий коллекцию иерархических терминов. Группа [может] содержать несколько наборов.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Наборы списков](../api/termstore-group-list-sets.md)|коллекция [microsoft.graph.termStore.set] | Возвращает список наборов, содержащихся в [группе] магазина [терминов.] |
|[Создание набора](../api/termstore-set-post.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Создание нового объекта набора в магазине [терминов.]|
|[Создание термина](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Создание нового [объекта терминов] в магазине [терминов.]|
|[Набор](../api/termstore-set-get.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)| Получить объект набора в магазине [терминов.]|
|[Получить термин](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)| Получить объект [терминов] в магазине [терминов.]|
|[Набор обновлений](../api/termstore-set-update.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Обновление свойств установленного объекта в магазине [терминов.]|
|[Удалить набор](../api/termstore-set-delete.md)|Нет.|Удаляет объект набора в магазине [терминов.]|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания набора. Только для чтения.|
|description|Строка|Описание, которое дает сведения об использовании термина.|
|id|Строка|Уникальный идентификатор. Только для чтения.|
|локализованные имена|[коллекция microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md)|Имя набора для каждого языкаTag.|
|properties|[коллекция microsoft.graph.keyValue](../resources/keyvalue.md)|Настраиваемые свойства для набора.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|children|[коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)|Children terms of set in term [store.]|
|parentGroup|[microsoft.graph.termStore.group](../resources/termstore-group.md)|Родительская [группа,] которая содержит набор.|
|отношения|[коллекция microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Указывает, какие термины были закреплены или повторноиспользовались непосредственно под набором.|
|термины|[коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)|Все условия под набором.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.set",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "String (identifier)",
  "localizedNames": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedName"
    }
  ],
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "properties": [
    {
      "@odata.type": "microsoft.graph.termStore.keyValue"
    }
  ]
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[магазин]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[термин]: ../resources/termstore-term.md


<!--
{
  "type": "#page.annotation",
  "description": "TermSet is the entity containing the particular taxonomy for a tenant",
  "keywords": "termSet,facet,resource",
  "section": "documentation",
  "tocPath": "TermSet",
  "tocBookmarks": {
    "Resources/termStore.set&quot;: &quot;#"
  },
  "suppressions": []
}
-->


