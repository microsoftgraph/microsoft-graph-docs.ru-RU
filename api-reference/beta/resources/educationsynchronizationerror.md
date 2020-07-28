---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 59650bc56554b9bd4dd7135ae44d53e153c159f8
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434839"
---
# <a name="educationsynchronizationerror-resource-type"></a>Тип ресурса educationSynchronizationError

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.

## <a name="methods"></a>Методы

| Метод                                                                     | Возвращаемый тип                                  | Описание                                                           |
| :------------------------------------------------------------------------- | :------------------------------------------- | :-------------------------------------------------------------------- |
| [Получение ошибок синхронизации](../api/educationsynchronizationerrors-get.md) | Коллекция **educationSynchronizationError** | Возвращает список ошибок синхронизации, связанных с профилем. |

## <a name="properties"></a>Свойства

| Свойство             | Тип           | Описание                                                     |
| :------------------- | :------------- | :-------------------------------------------------------------- |
| id                   | Строка         | Уникальный идентификатор ресурса. (только для чтения)             |
| ентритипе            | Строка         | Представляет объект синхронизации (School, section, Student, преподаватель). |
| errorCode            | String         | Представляет код ошибки для этой ошибки.                       |
| Ошибк         | Строка         | Содержит описание ошибки.                            |
| жоинингвалуе         | Строка         | Уникальный идентификатор для записи.                            |
| recordedDateTime     | DateTimeOffset | Время возникновения ошибки.                           |
| репортаблеидентифиер | Строка         | Идентификатор этой записи об ошибке.                             |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
  "id": "String",
  "entryType": "String",
  "errorCode": "String",
  "errorMessage": "String",
  "joiningValue": "String",
  "recordedDateTime": "DateTimeOffset",
  "reportableIdentifier": "String"
}
```
