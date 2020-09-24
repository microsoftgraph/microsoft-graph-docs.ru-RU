---
title: Тип ресурса хранилища
description: Представляет банк терминов таксономии.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: de8b0c004da804a4d9a617eec20de22c51e98108
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258438"
---
# <a name="store-resource-type"></a>Тип ресурса хранилища

Пространство имен: Microsoft. Graph. банка

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет банк терминов таксономии.

Наследуется от [объекта Entity](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание
|:---|:---|:---
|[Перечисление групп](../api/termstore-list-groups.md)|Коллекция [Microsoft. Graph. банка терминов Microsoft. Graph.](../resources/termstore-group.md)| Получение групп из доступных в объекте банка терминов.|
|[Получение хранилища](../api/termstore-store-get.md) | [Microsoft. Graph. Банк. Банк.](../resources/termstore-store.md) | Чтение свойств и связей объекта банка терминов.
|[Обновление хранилища](../api/termstore-store-update.md) | [Microsoft. Graph. Банк. Банк.](../resources/termstore-store.md) | Обновление свойств объекта банка терминов.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание
|:---|:---|:---
|дефаултлангуажетаг | Строка | Язык банка терминов по умолчанию.
|id|Строка | Уникальный идентификатор банка терминов. Только для чтения.
|лангуажетагс | Коллекция String | Список языков для банка терминов.

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание
|:---|:---|:---
|groups |Коллекция [Microsoft. Graph. банка терминов Microsoft. Graph.](../resources/termstore-group.md) | Коллекция всех групп, доступных в банке терминов.
|предваритель | Коллекция [Microsoft. Graph. Банк. Set для Microsoft. Graph.](../resources/termstore-set.md) | Коллекция всех наборов, доступных в банке терминов.


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



