---
title: Тип ресурса Усеррегистратионкаунт
description: Представляет счетчик регистраций и состояние для пользователей в клиенте.
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 3e3a5e7e3925f5528d5ce73a15233cea8e50eebd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524185"
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

## <a name="json-representation"></a>Представление JSON

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

