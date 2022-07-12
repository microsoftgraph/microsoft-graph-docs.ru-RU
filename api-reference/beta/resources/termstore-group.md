---
author: mohitpcad
title: Тип ресурса группы
doc_type: resourcePageType
description: Представляет группу, используемую в хранилище терминов.
ms.localizationpriority: medium
ms.prod: taxonomy
ms.openlocfilehash: 3bd7f818cf9e38dcffcba9fac0c93b248d1d10d9
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732683"
---
# <a name="group-resource-type"></a>Тип ресурса группы

Пространство имен: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Представляет группу, используемую в хранилище [терминов](../resources/termstore-store.md). Группа — это логическая иерархия, содержащая под ней коллекцию наборов. 

Наследует [от сущности](../resources/entity.md).


## <a name="methods"></a>Методы

| Метод                                                   | Тип возвращаемых данных       |    Описание|
|:---------------------------------------------------------|:------------------|:---------------------|
| [Создание группы](../api/termstore-group-post.md)                     | [microsoft.graph.termStore.group] | Создайте группу в хранилище [терминов].|
| [Получение группы](../api/termstore-group-get.md)                           | [microsoft.graph.termStore.group] | Получение данных группы в хранилище [терминов].|
| [Удаление группы](../api/termstore-group-delete.md)                     | Нет |  Удаление группы в хранилище [терминов].|

## <a name="properties"></a>Свойства

| Свойство             | Тип               | Описание|
|:---------------------|:-------------------|:------------------------------------|
| createdDateTime      | DateTimeOffset     | Дата и время создания группы. Только для чтения.|
| description          | string             | Описание, содержащее сведения об использовании термина.|
| id                   | string             | Уникальный идентификатор группы. Только для чтения.|
| displayName          | string             | Имя группы.|
| scope                | string              | Возвращает тип группы. Возможные значения: `global`, `system` и `siteCollection`.|
| parentSiteId         | String             | Идентификатор родительского сайта этой группы.|

## <a name="relationships"></a>Связи
| Связь       | Тип                        | Описание|
|:-------------------|:----------------------------|:--------------------------|
| Задает           | [Коллекция microsoft.graph.termStore.set][] | Все наборы в группе в банках [терминов].|

## <a name="json-representation"></a>Представление JSON

Ниже приведено представление ресурса группы в **формате** JSON.
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
[Магазин]: ../resources/termstore-store.md
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


