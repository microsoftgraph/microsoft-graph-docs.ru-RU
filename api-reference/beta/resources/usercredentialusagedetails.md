---
title: Тип ресурса userCredentialUsageDetails
description: Представляет использование самостоятельного сброса пароля для данного клиента.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3992272aa6917aa43d2ffdb4c4c980b88fc60e7e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159820"
---
# <a name="usercredentialusagedetails-resource-type"></a>Тип ресурса userCredentialUsageDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет использование самостоятельного сброса пароля для данного клиента. Сведения включают сведения о пользователе, состояние сброса и причину сбоя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md) | userCredentialUsageDetails | Чтение свойств и связей объекта userCredentialUsageDetails. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| authMethod | string | Представляет метод проверки подлинности, используемый пользователем. Возможные значения: , , , , (используется только для самостоятельного сброса `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` пароля), `appNotification` , и `appCode` `alternateMobileCall` (поддерживается только при регистрации). |
| eventDateTime | DateTimeOffset | Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
| failureReason | String | Предоставляет причину сбоя для соответствующего рабочего процесса сброса или регистрации. |
| feature | string | Возможные значения: `registration` и `reset` . |
| id | String | Только для чтения. Уникальный идентификатор действия. Только для чтения.|
| isSuccess | Boolean | Указывает на успешность или сбой рабочего процесса. |
| userDisplayName | String | Имя пользователя, который выполняет рабочий процесс сброса или регистрации. |
| userPrincipalName | String | Имя пользователя, который выполняет рабочий процесс сброса или регистрации. |

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

