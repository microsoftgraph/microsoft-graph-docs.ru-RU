---
title: тип ресурса хранения
description: Представляет хранилище терминов таксономии.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 840e22fc3031787cbc550f0ee0e32d5e6243bed9
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514983"
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
|LanguageTags | Коллекция объектов string | Список языков для магазина терминов.|

## <a name="relationships"></a>Связи
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



