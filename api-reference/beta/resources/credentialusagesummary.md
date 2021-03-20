---
title: тип ресурса credentialUsageSummary
description: Представляет текущее состояние того, сколько пользователей в организации используют возможности сброса паролей самообслуживки.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 9db31a0d0397f1394a342fb52796a1bec37bae36
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941832"
---
# <a name="credentialusagesummary-resource-type"></a>тип ресурса credentialUsageSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние того, сколько пользователей в организации используют возможности сброса паролей самообслуживки.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md) | credentialUsageSummary | Чтение свойств и связей объекта credentialUsageSummary. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| authMethod | useAuthMethod | Представляет метод проверки подлинности, используемый пользователем. Возможные значения: , , , , (только используется для самообслуживки сброс `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` пароля), , , ( `appNotification` `appCode` `alternateMobileCall` поддерживается `fido` `appPassword` `unknownFutureValue` только в регистрации), , , . |
| failureActivityCount | Int64 | Обеспечивает количество сбойных сбросов или данных регистрации. |
| функция | featureType | Определяет функцию для отчета. Возможные значения: `registration`, `reset`, `unknownFutureValue`. |
| id | Строка | Уникальный идентификатор для этого действия. Только для чтения. |
| successfulActivityCount | Int64 | Обеспечивает количество успешных регистраций или сбросов. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "successfulActivityCount":"Int64",
  "failureActivityCount": "Int64",
  "authMethod": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUsageSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

