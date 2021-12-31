---
title: тип ресурса applicationSignInDetailedSummary
description: Представляет сводку регистрации приложения.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1c0f07f40ee2b03dd350ea918dc0b1fe43a1b1c5
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647143"
---
# <a name="applicationsigninsummary-resource-type"></a>тип ресурса applicationSignInSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сводку регистрации приложения.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md) | [applicationSignInSummary](applicationsigninsummary.md) | Ознакомьтесь с свойствами и отношениями **объекта applicationSignInSummary.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String|Имя приложения, в которое пользователь подписался.|
|failedSignInCount|Int64|Количество неудачных входов, сделанных приложением.|
|successPercentage|Int32|Процент успешных входов, сделанных приложением.|
|successfulSignInCount|Int64|Количество успешных входов, сделанных приложением.|
<!--Hiding this because it's not in the metadata nor in public response objects
|appId|String|  Identifier of the application that the user signed into.|
-->

## <a name="relationships"></a>Отношения
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


