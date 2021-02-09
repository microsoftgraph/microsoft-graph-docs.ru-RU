---
title: Тип ресурса connectionOperation
description: Описывает состояние асинхронного запроса на создание схемы подключения Поиска (Майкрософт).
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e17b1f55b00fd7b9bdc69eb7a7a34d3453ab332d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158305"
---
# <a name="connectionoperation-resource-type"></a>Тип ресурса connectionOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает состояние асинхронного запроса на создание схемы подключения Поиска [(Майкрософт).](schema.md)

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get connectionOperation](../api/connectionoperation-get.md) | [connectionOperation](connectionoperation.md) | Чтение свойств объекта connectionOperation. |

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                       |
|:---------|:------------------------------|:----------------------------------|
| error    | [errorDetail](errordetail.md) | Если `status` это `failed` так, предоставляет дополнительные сведения об ошибке, которая привела к сбою. |
| id       | String                        | Уникальный идентификатор для connectionOperation. Только для чтения. |
| status   | string                        | Указывает состояние асинхронной операции. Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
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


