---
title: Тип ресурса credentialUserRegistrationCount
description: Представляет текущее состояние регистрации пользователей в организации для самостоятельного сброса паролей и многофакторной проверки подлинности.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 521c8eca7c3233000bf04f2324e8990fd25c55f6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159922"
---
# <a name="credentialuserregistrationcount-resource-type"></a>Тип ресурса credentialUserRegistrationCount

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние регистрации пользователей в организации для самостоятельного сброса паролей и многофакторной проверки подлинности.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md) | Коллекция credentialUserRegistrationCount | Фиксируйте текущее состояние регистрации пользователей в организации для самостоятельного сброса паролей и многофакторной проверки подлинности (MFA). |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| id | String | Уникальный идентификатор действия. Только для чтения. |
| totalUserCount | Int64 | Предоставляет общее количество пользователей в клиенте. |
| userRegistrationCounts | [Коллекция userRegistrationCount](userregistrationcount.md) | Коллекция сведений о регистрации и состоянии для пользователей в клиенте. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
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

