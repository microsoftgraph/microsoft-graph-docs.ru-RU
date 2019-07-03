---
title: Тип ресурса Кредентиалусеррегистратионкаунт
description: Представляет текущее состояние количества пользователей в вашей организации, зарегистрированных для самостоятельного сброса паролей и возможности многофакторной проверки подлинности.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 42c722b04493767d3dbcaf713157d931569d8c32
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487607"
---
# <a name="credentialuserregistrationcount-resource-type"></a>Тип ресурса Кредентиалусеррегистратионкаунт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние количества пользователей в вашей организации, зарегистрированных для самостоятельного сброса паролей и возможности многофакторной проверки подлинности.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Жеткредентиалусеррегистратионкаунт](../api/reportroot-getcredentialuserregistrationcount.md) | Коллекция Кредентиалусеррегистратионкаунт | Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA). |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| id | String | Уникальный идентификатор действия. Только для чтения. |
| Тоталусеркаунт | Int64 | Предоставляет общее число пользователей в клиенте. |
| Усеррегистратионкаунтс | Коллекция [усеррегистратионкаунт](userregistrationcount.md) | Коллекция счетчиков регистрации и сведений о состоянии для пользователей в клиенте. |

## <a name="relationships"></a>Отношения

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