---
title: Тип ресурса Кредентиалусажесуммари
description: Представляет текущее состояние того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 311f89b67549e6bc373029aef82c88ca0e592f3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050096"
---
# <a name="credentialusagesummary-resource-type"></a>Тип ресурса Кредентиалусажесуммари

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [жеткредентиалусажесуммари](../api/reportroot-getcredentialusagesummary.md) | кредентиалусажесуммари | Чтение свойств и связей объекта Кредентиалусажесуммари. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| аусмесод | string | Представляет способ проверки подлинности, используемый пользователем. Возможные значения: `email` ,,,, `mobileSMS` `mobileCall` `officePhone` `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode` и  `alternateMobileCall` (поддерживается только для регистрации). |
| фаилуреактивитикаунт | Int64 | Предоставляет количество неудачных сбросов или регистрационных данных. |
| состав | string | Определяет компонент для отчета. Возможные значения: `registration` и `reset` . |
| id | Строка | Уникальный идентификатор действия. Только для чтения. |
| сукцессфулактивитикаунт | Int64 | Предоставляет количество успешных регистраций или сбросов. |

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

