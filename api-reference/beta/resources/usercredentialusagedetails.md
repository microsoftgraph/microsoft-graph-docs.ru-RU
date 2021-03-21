---
title: тип ресурса userCredentialUsageDetails
description: Представляет использование сброса пароля самообслуживателя для данного клиента.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: deb5c93570a9921bc1830bfcb0772d643eed68b7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958733"
---
# <a name="usercredentialusagedetails-resource-type"></a>тип ресурса userCredentialUsageDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет использование сброса пароля самообслуживателя для данного клиента. Сведения включают сведения о пользователях, состояние сброса и причину сбоя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список пользователейCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md) | userCredentialUsageDetails | Чтение свойств и связей объекта userCredentialUsageDetails. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| authMethod | useAuthMethod | Представляет метод проверки подлинности, используемый пользователем. Возможные значения: , , , , (только используется для самообслуживки сброс `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` пароля), `appNotification` , , ( `appCode` `alternateMobileCall` поддерживается только в регистрации), `fido` , `appPassword` ,`unknownFutureValue` |
| eventDateTime | DateTimeOffset | Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. |
| failureReason | String | Предоставляет причину сбоя для соответствующего рабочего процесса сброса или регистрации. |
| функция | featureType | Возможные значения: `registration`, `reset`, `unknownFutureValue`. |
| id | String | Только для чтения. Уникальный идентификатор для этого действия. Только для чтения.|
| isSuccess | Boolean | Указывает на успешность или сбой рабочего процесса. |
| userDisplayName | String | Имя пользователя, который выполняет рабочий процесс сброса или регистрации. |
| userPrincipalName | String | Основное имя пользователя, который выполняет рабочий процесс сброса или регистрации. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "isSuccess" : true,
  "authMethod": "string",
  "failureReason": "String",
  "eventDateTime" : "DateTimeOffset"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userCredentialUsageDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

