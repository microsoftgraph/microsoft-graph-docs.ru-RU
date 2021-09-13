---
title: тип ресурса хранения
description: Представляет хранилище терминов таксономии.
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: c94c0edb6589bd467676ac42294ead8416e829df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084043"
---
# <a name="store-resource-type"></a>тип ресурса хранения

Пространство имен: microsoft.graph.termStore

Представляет хранилище терминов таксономии.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление групп](../api/termstore-list-groups.md)|[коллекция microsoft.graph.termStore.group](../resources/termstore-group.md)| Получите группы, доступные в объекте магазина терминов.|
|[Get store](../api/termstore-store-get.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | Ознакомьтесь с свойствами и отношениями объекта хранения терминов.|
|[Магазин обновлений](../api/termstore-store-update.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | Обновление свойств объекта магазина терминов.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|defaultLanguageTag | Строка | Язык по умолчанию магазина терминов.|
|id|Строка | Уникальный идентификатор магазина терминов. Только для чтения.|
|LanguageTags | Коллекция String | Список языков для магазина терминов.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|groups |[коллекция microsoft.graph.termStore.group](../resources/termstore-group.md) | Коллекция всех групп, доступных в магазине терминов.|
|наборы | [коллекция microsoft.graph.termStore.set](../resources/termstore-set.md) | Коллекция всех наборов, доступных в магазине терминов.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.store",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.store",
  "id": "String (identifier)",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "TermStore is the top-level entity used for managing taxonomy for a client",
  "keywords": "termStore,facet,resource",
  "section": "documentation",
  "tocPath": "TermStore",
  "tocBookmarks": {
    "Resources/termStore.store": "#"
  },
  "suppressions": []
}
-->



