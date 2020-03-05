---
title: Тип ресурса Коннектионоператион
description: Описывает состояние асинхронного запроса для создания схемы подключения поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 21d962bbbfee64c51f11cf1ac3f5e7de2c0497e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507487"
---
# <a name="connectionoperation-resource-type"></a>Тип ресурса Коннектионоператион

Пространство имен: Microsoft. Graph

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
| error    | [еррордетаил](errordetail.md) | Если `status` это `failed`так, предоставляет дополнительные сведения об ошибке, вызвавшей сбой. |
| id       | Строка                        | Уникальный идентификатор для Коннектионоператион. Только для чтения. |
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
