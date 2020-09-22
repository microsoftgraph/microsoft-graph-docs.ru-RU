---
title: Тип ресурса Усеррегистратионкаунт
description: Представляет счетчик регистраций и состояние для пользователей в клиенте.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 5aa86a0b490ddb2cd68a504f5a4879f922fa0cf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057829"
---
# <a name="userregistrationcount-resource-type"></a>Тип ресурса Усеррегистратионкаунт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет счетчик регистраций и состояние для пользователей в клиенте.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| регистратионкаунт | Int64 | Предоставляет счетчик регистраций для клиента. |
| регистратионстатус | String | Представляет состояние регистрации пользователя. Возможные значения: `registered` , `enabled` , `capable` и `mfaRegistered` . |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userRegistrationCount",
  "baseType": null
}-->

```json
{ 
  "registrationStatus":"String", 
  "registrationCount": 23423
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

