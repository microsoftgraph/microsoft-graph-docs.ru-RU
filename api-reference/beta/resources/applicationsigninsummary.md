---
title: Тип ресурса applicationSignInDetailedSummary
description: Представляет сводку по входу в приложение.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 454c4e2e9e57b61194e6f3e6970e5db1ea414369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137412"
---
# <a name="applicationsigninsummary-resource-type"></a>Тип ресурса applicationSignInSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сводку по входу в приложение.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение applicationSignInSummary](../api/applicationsigninsummary-get.md) | [applicationSignInSummary](applicationsigninsummary.md) | Чтение свойств и связей объекта **applicationSignInSummary.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String|Имя приложения, в которое вписались пользователи.|
|appId|String|  ИД приложения, подписанного пользователем i nto.|
|failedSignInCount|Int64|Количество неудачных входов в приложение.|
|successPercentage|Int32|Процент успешных входов, сделанных приложением.|
|successfulSignInCount|Int64|Количество успешных входов, сделанных приложением.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInSummary"
}-->

```json
{
  "appDisplayName": "String",
  "appId": "String (identifier)",
  "failedSignInCount": 1024,
  "successPercentage": 1024,
  "successfulSignInCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


