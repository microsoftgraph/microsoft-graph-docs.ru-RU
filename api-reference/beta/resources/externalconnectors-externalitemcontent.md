---
title: тип ресурса externalItemContent
description: Содержимое элемента, индексироваться с помощью Поиск (Майкрософт) подключения.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 36ca1d19e9be37d7c47c9195fc2c63f677673c0e
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2022
ms.locfileid: "63560103"
---
# <a name="externalitemcontent-resource-type"></a>тип ресурса externalItemContent

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержимое [externalItem,](externalconnectors-externalitem.md) индексироваться с помощью Поиск (Майкрософт) [подключения](externalconnectors-externalconnection.md).

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| значение    | String | Содержимое для externalItem. Обязательное.                                                 |
| type     | String | Тип контента в свойстве значения. Возможные значения: `text` и `html`. Это типы контента, поддерживаемые индексером, а не разрешенные типы расширения файлов. Обязательный. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
}-->

```json
{
  "value": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItemContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
