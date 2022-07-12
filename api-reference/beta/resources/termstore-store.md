---
title: тип ресурса store
description: Представляет хранилище терминов таксономии.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: f1b38c9fb826ce430614d44a7b41ed1712523481
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735938"
---
# <a name="store-resource-type"></a>тип ресурса store

Пространство имен: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет хранилище терминов таксономии.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание
|:---|:---|:---
|[Список групп](../api/termstore-list-groups.md)|[Коллекция microsoft.graph.termStore.group](../resources/termstore-group.md)| Получение групп из доступных в объекте банка терминов.|
|[Получение хранилища](../api/termstore-store-get.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | Чтение свойств и связей объекта банка терминов.
|[Обновление хранилища](../api/termstore-store-update.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | Обновление свойств объекта банка терминов.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание
|:---|:---|:---
|defaultLanguageTag | Строка | Язык по умолчанию для банка терминов.
|id|String | Уникальный идентификатор банка терминов. Только для чтения.
|languageTags | Коллекция строк | Список языков для банка терминов.

## <a name="relationships"></a>Связи
|Связь|Тип|Описание
|:---|:---|:---
|groups |[Коллекция microsoft.graph.termStore.group](../resources/termstore-group.md) | Коллекция всех групп, доступных в хранилище терминов.
|Задает | [Коллекция microsoft.graph.termStore.set](../resources/termstore-set.md) | Коллекция всех наборов, доступных в хранилище терминов.


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



