---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2af4ef9f17452714373d42b67af6e87a7f87fe1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989650"
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
| id                   | String         | Уникальный идентификатор ресурса. (только для чтения)             |
| ентритипе            | String         | Представляет объект синхронизации (School, section, Student, преподаватель). |
| errorCode            | String         | Представляет код ошибки для этой ошибки.                       |
| Ошибк         | String         | Содержит описание ошибки.                            |
| жоинингвалуе         | String         | Уникальный идентификатор для записи.                            |
| recordedDateTime     | DateTimeOffset | Время возникновения ошибки.                           |
| репортаблеидентифиер | String         | Идентификатор этой записи об ошибке.                             |

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


