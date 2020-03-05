---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d46d1160ae59174d9fcb4df89559531e3a032e55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500326"
---
# <a name="educationsynchronizationerror-resource-type"></a>Тип ресурса educationSynchronizationError

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Получение ошибок синхронизации](../api/educationsynchronizationerrors-get.md) | Коллекция **educationSynchronizationError**| Возвращает список ошибок синхронизации, связанных с профилем. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **ентритипе** | строка |  Представляет объект синхронизации (School, section, Student, преподаватель).       |
| **errorCode** | строка |  Представляет код ошибки для этой ошибки.         |
| **Ошибк** | строка |  Содержит описание ошибки.        |
| **жоинингвалуе** | строка |  Уникальный идентификатор для записи.         |
| **recordedDateTime** | DateTimeOffset | Время возникновения ошибки.         |
| **репортаблеидентифиер** | строка | Идентификатор этой записи об ошибке.       |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
