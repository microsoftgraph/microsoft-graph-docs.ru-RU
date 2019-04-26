---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3c512f921e77468bb30e5109eec29afa9b395b7e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340536"
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
