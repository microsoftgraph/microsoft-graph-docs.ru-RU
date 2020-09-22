---
title: Тип ресурса Коннектионоператион
description: Описывает состояние асинхронного запроса для создания схемы подключения поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aed9574ba6fd5e8b2c47b38ee4eebb3326cf2a37
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027190"
---
# <a name="connectionoperation-resource-type"></a>Тип ресурса Коннектионоператион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние асинхронного запроса для создания [схемы](schema.md)подключения поиска Microsoft Search.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Коннектионоператион](../api/connectionoperation-get.md) | [коннектионоператион](connectionoperation.md) | Чтение свойств объекта Коннектионоператион. |

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                       |
|:---------|:------------------------------|:----------------------------------|
| error    | [еррордетаил](errordetail.md) | Если `status` это так `failed` , предоставляет дополнительные сведения об ошибке, вызвавшей сбой. |
| id       | String                        | Уникальный идентификатор для Коннектионоператион. Только для чтения. |
| status   | string                        | Указывает состояние асинхронной операции. Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`. |

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.errorDetail"},
  "id": "String (identifier)",
  "status": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectionOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


