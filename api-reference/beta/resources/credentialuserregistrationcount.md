---
title: Тип ресурса Кредентиалусеррегистратионкаунт
description: Представляет текущее состояние количества пользователей в вашей организации, зарегистрированных для самостоятельного сброса паролей и возможности многофакторной проверки подлинности.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: c5fb3588c7d06f726c71c81279c0994fd0de4019
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050089"
---
# <a name="credentialuserregistrationcount-resource-type"></a>Тип ресурса Кредентиалусеррегистратионкаунт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние количества пользователей в вашей организации, зарегистрированных для самостоятельного сброса паролей и возможности многофакторной проверки подлинности.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [жеткредентиалусеррегистратионкаунт](../api/reportroot-getcredentialuserregistrationcount.md) | Коллекция Кредентиалусеррегистратионкаунт | Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA). |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| id | Строка | Уникальный идентификатор действия. Только для чтения. |
| тоталусеркаунт | Int64 | Предоставляет общее число пользователей в клиенте. |
| усеррегистратионкаунтс | Коллекция [усеррегистратионкаунт](userregistrationcount.md) | Коллекция счетчиков регистрации и сведений о состоянии для пользователей в клиенте. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "totalUserCount" : 23123,
  "userRegistrationCounts" :
  [
    { "registrationStatus":"registered", "registrationCount": 23423 },
    { "registrationStatus":"enabled", "registrationCount": 4234 },
    { "registrationStatus":"capable", "registrationCount": 323 },
    { "registrationStatus":"mfaRegistered", "registrationCount": 33 }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

