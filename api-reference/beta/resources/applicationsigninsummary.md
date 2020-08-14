---
title: Тип ресурса Аппликатионсигниндетаиледсуммари
description: Представляет сводку по входу в приложение.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b67eae972137e168218070013952dae4690bf95a
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46673721"
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
