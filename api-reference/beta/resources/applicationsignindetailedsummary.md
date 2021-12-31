---
title: тип ресурса applicationSignInDetailedSummary — API Graph Microsoft
description: Представляет подробную сводку регистрации приложения.
ms.localizationpriority: medium
author: sureshja
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b929e35904af0ddec506a8b1b47e502456adb3c6
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647171"
---
# <a name="applicationsignindetailedsummary-resource-type"></a>тип ресурса applicationSignInDetailedSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробную сводку регистрации приложения.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md) | [коллекция applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Получение **объектов applicationSignInDetailedSummary.** |
| [Получение applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Ознакомьтесь с свойствами и отношениями **объекта applicationSignInDetailedSummary.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|aggregatedEventDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|appDisplayName|String|Имя приложения, в которое пользователь вписались.|
|appId|String|ID приложения, в которое пользователь вписался.|
|id|String| Уникальный ID, представляющий действие входного знака.|
|signInCount|Int64|Количество входов, сделанных приложением.|
|status|[signInStatus](signinstatus.md)|Сведения о состоянии регистрации.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
}-->

```json
{
  "aggregatedEventDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "id": "String (identifier)",
  "signInCount": 1024,
  "status": {"@odata.type": "microsoft.graph.signInStatus"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


