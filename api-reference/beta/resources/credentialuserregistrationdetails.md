---
title: тип ресурса credentialUserRegistrationDetails
description: Представляет сведения об использовании сброса пароля самообслуживления и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ac5712bf3c0d396f7ddc84c4812b4e1ed7090355
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941815"
---
# <a name="credentialuserregistrationdetails-resource-type"></a>тип ресурса credentialUserRegistrationDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об использовании сброса пароля самообслуживления и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей. Сведения включают сведения о пользователях, состояние регистрации и используемый метод проверки подлинности.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md) | коллекция credentialUserRegistrationDetails | Получите список объектов [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) для данного клиента.
 |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| authMethods | registrationAuthMethod collection | Представляет метод проверки подлинности, зарегистрированный пользователем. Возможные значения: , , , (только используется для самообслуживки сброс `email` `mobilePhone` `officePhone`  `securityQuestion` пароля), , , ( `appNotification`  `appCode` `alternateMobilePhone` поддерживается  `fido`  `appPassword`  `unknownFutureValue` только в регистрации), , , . |
| id | Строка | Уникальный идентификатор для этого действия. Только для чтения.|
| isCapable | Boolean | Указывает, готов ли пользователь выполнять сброс пароля самообслуживки или MFA. |
| isEnabled | Boolean | Указывает, включен ли пользователь для выполнения сброса пароля самообслуживки. |
| isMfaRegistered | Boolean | Указывает, зарегистрирован ли пользователь для MFA. |
| isRegistered | Boolean | Указывает, зарегистрировал ли пользователь какие-либо методы проверки подлинности для сброса пароля самообслуживления. |
| userDisplayName | String | Предоставляет имя пользователя соответствующего пользователя. |
| userPrincipalName | String | Предоставляет основное имя пользователя соответствующего пользователя. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "authMethods": ["string"],
  "isRegistered" : false,
  "isEnabled" : true,
  "isCapable" : false,
  "isMfaRegistered" : true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


