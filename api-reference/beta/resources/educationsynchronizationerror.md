---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525145"
---
# <a name="educationsynchronizationerror-resource-type"></a>Тип ресурса educationSynchronizationError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Получение ошибки синхронизации](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError** коллекции| Возвращает список ошибок синхронизации службы, связанные с профилем. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **entryType** | string |  Представляет сущности синхронизации (школа, раздел, учебы, преподаватель).       |
| errorCode | string |  Представляет код ошибки для этой ошибки.         |
| **ErrorMessage** | string |  Содержит описание ошибки.        |
| **joiningValue** | string |  Уникальный идентификатор для записи.         |
| recordedDateTime | DateTimeOffset | Время возникновения этой ошибки.         |
| **reportableIdentifier** | string | Идентификатор элемента в этой записи об ошибках.       |

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
