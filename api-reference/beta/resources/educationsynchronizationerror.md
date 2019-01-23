---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 397ac305fcacd789174c05ea36ab026826227475
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425815"
---
# <a name="educationsynchronizationerror-resource-type"></a>Тип ресурса educationSynchronizationError

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Получение ошибки синхронизации](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError** коллекции| Возвращает список ошибок синхронизации службы, связанные с профилем. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **entryType** | string |  Представляет сущности синхронизации (школа, раздел, учебы, преподаватель).       |
| **errorCode** | string |  Представляет код ошибки для этой ошибки.         |
| **сообщение об ошибке** | string |  Содержит описание ошибки.        |
| **joiningValue** | string |  Уникальный идентификатор для записи.         |
| **recordedDateTime** | DateTimeOffset | Время возникновения этой ошибки.         |
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
