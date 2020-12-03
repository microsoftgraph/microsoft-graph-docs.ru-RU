---
title: Тип ресурса Аппликатионсигниндетаиледсуммари
description: Представляет сводку по входу в приложение.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: abe2d8524d2ef23885285bacc0c953057035f54d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523814"
---
# <a name="applicationsigninsummary-resource-type"></a>Тип ресурса Аппликатионсигнинсуммари

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сводку по входу в приложение.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Аппликатионсигнинсуммари](../api/applicationsigninsummary-get.md) | [аппликатионсигнинсуммари](applicationsigninsummary.md) | Чтение свойств и связей объекта **аппликатионсигнинсуммари** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|appDisplayName|String|Имя приложения, в которое пользователь выполнил вход.|
|appId|String|  Идентификатор приложения, выполнившего вход пользователя.|
|фаиледсигнинкаунт|Int64|Количество неудачных операций входа, выполненных приложением.|
|сукцессперцентаже|Int32|Процент успешных входов, выполненных приложением.|
|сукцессфулсигнинкаунт|Int64|Количество успешных входов, выполненных приложением.|

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


