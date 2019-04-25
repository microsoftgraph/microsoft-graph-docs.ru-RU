---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542968"
---
# <a name="educationsynchronizationerror-resource-type"></a>Тип ресурса educationSynchronizationError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Получение ошибок синхронизации](../api/educationsynchronizationerrors-get.md) | Коллекция **educationSynchronizationError**| Возвращает список ошибок синхронизации, связанных с профилем. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Ентритипе** | string |  Представляет объект синхронизации (School, section, Student, преподаватель).       |
| **Коде** | string |  Представляет код ошибки для этой ошибки.         |
| **Ошибк** | string |  Содержит описание ошибки.        |
| **Жоинингвалуе** | string |  Уникальный идентификатор для записи.         |
| **recordedDateTime** | DateTimeOffset | Время возникновения ошибки.         |
| **Репортаблеидентифиер** | string | Идентификатор этой записи об ошибке.       |

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
