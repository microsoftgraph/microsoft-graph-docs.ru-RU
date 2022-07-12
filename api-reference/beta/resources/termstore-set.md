---
title: Задать тип ресурса
description: Представляет набор в хранилище терминов.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: b9374c1d41ef713b6edfeb3dd0ec4614b5562c2a
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734230"
---
# <a name="set-resource-type"></a>Задать тип ресурса

Пространство имен: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор, используемый в хранилище [терминов]. Набор представляет единицу, содержащую коллекцию иерархических терминов. Группа [может] содержать несколько наборов.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Наборы списков](../api/termstore-group-list-sets.md)|коллекция [microsoft.graph.termStore.set] | Возвращает список наборов, содержащихся в [группе] банка [терминов]. |
|[Создание набора](../api/termstore-set-post.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Создайте объект набора в хранилище [терминов].|
|[Создание термина](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Создайте объект [термина] в хранилище [терминов].|
|[Получить набор](../api/termstore-set-get.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)| Получение объекта set в хранилище [терминов].|
|[Получение термина](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)| Получение объекта [термина] в хранилище [терминов].|
|[Набор обновлений](../api/termstore-set-update.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Обновление свойств объекта set в хранилище [терминов].|
|[Удалить набор](../api/termstore-set-delete.md)|Нет|Удаляет объект набора в хранилище [терминов].|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания набора. Только для чтения.|
|description|String|Описание, содержащее сведения об использовании термина.|
|id|String|Уникальный идентификатор. Только для чтения.|
|localizedNames|[Коллекция microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md)|Имя набора для каждого языкового тега.|
|properties|[Коллекция microsoft.graph.keyValue](../resources/keyvalue.md)|Настраиваемые свойства для набора.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|children|[Коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)|Дочерние условия набора в банках [терминов].|
|parentGroup|[microsoft.graph.termStore.group](../resources/termstore-group.md)|Родительская [группа] , содержащая набор.|
|Отношения|[Коллекция microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Указывает, какие термины были закреплены или повторно использоваться непосредственно в наборе.|
|Условия|[Коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)|Все термины в наборе.|

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
[store]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[Термин]: ../resources/termstore-term.md


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


