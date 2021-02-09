---
title: Тип ресурса credentialUserRegistrationDetails
description: Представляет сведения об использовании самостоятельного сброса паролей и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c7e45b186e1ef7a3a96115f408cb5a0992e538fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159908"
---
# <a name="credentialuserregistrationdetails-resource-type"></a>Тип ресурса credentialUserRegistrationDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об использовании самостоятельного сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей. Сведения включают сведения о пользователе, состояние регистрации и используемый метод проверки подлинности.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md) | Коллекция credentialUserRegistrationDetails | Получите список объектов [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) для данного клиента.
 |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| authMethods | коллекция registrationAuthMethod | Представляет метод проверки подлинности, зарегистрированный пользователем. Возможные значения: , , , (используется только для самостоятельного сброса `email` `mobilePhone` `officePhone` `securityQuestion` пароля), `appNotification` , и `appCode` `alternateMobilePhone` (поддерживается только при регистрации). |
| id | String | Уникальный идентификатор действия. Только для чтения.|
| isCapable | Boolean | Указывает, готов ли пользователь к самостоятельному сбросу пароля или MFA. |
| isEnabled | Boolean | Не сообщает, включен ли для пользователя самостоятельный сброс пароля. |
| isMfaRegistered | Boolean | Не сообщает, зарегистрирован ли пользователь для MFA. |
| isRegistered | Boolean | Указывает, зарегистрирован ли пользователь какие-либо методы проверки подлинности для самостоятельного сброса пароля. |
| userDisplayName | String | Предоставляет имя соответствующего пользователя. |
| userPrincipalName | String | Предоставляет имя основного пользователя соответствующего пользователя. |

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


