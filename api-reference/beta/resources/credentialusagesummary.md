---
title: Тип ресурса credentialUsageSummary
description: Представляет текущее состояние того, сколько пользователей в организации используют возможности самостоятельного сброса паролей.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 03ae7b4b03cf58301895e5246fa4cb86d1b79667
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157703"
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
| id | String | Уникальный идентификатор действия. Только для чтения. |
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

