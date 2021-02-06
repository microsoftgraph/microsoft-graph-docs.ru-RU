---
title: Тип ресурса credentialUsageSummary
description: Представляет текущее состояние того, сколько пользователей в организации используют возможности самостоятельного сброса паролей.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 43a17f91a1424d9ac8c0a388ef5404bbadf05189
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136286"
---
# <a name="credentialusagesummary-resource-type"></a>Тип ресурса credentialUsageSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние того, сколько пользователей в организации используют возможности самостоятельного сброса паролей.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md) | credentialUsageSummary | Чтение свойств и связей объекта credentialUsageSummary. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| authMethod | string | Представляет метод проверки подлинности, используемый пользователем. Возможные значения: , , , , (используется только для самостоятельного сброса `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` пароля), `appNotification` , и `appCode`  `alternateMobileCall` (поддерживается только для регистрации). |
| failureActivityCount | Int64 | Предоставляет количество неудачных сбросов или регистрационных данных. |
| feature | string | Определяет функцию для отчета. Возможные значения: `registration` и `reset` . |
| id | Строка | Уникальный идентификатор действия. Только для чтения. |
| successfulActivityCount | Int64 | Предоставляет количество успешных регистраций или сбросов. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "baseType": "",
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

