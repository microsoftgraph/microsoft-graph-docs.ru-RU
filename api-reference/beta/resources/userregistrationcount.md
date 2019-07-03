---
title: Тип ресурса Усеррегистратионкаунт
description: Представляет счетчик регистраций и состояние для пользователей в клиенте.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 43f151864f7ca996602e7bd2fc42f3fa4ba743d1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489507"
---
# <a name="userregistrationcount-resource-type"></a>Тип ресурса Усеррегистратионкаунт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет счетчик регистраций и состояние для пользователей в клиенте.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| Регистратионкаунт | Int64 | Предоставляет счетчик регистраций для клиента. |
| Регистратионстатус | String | Представляет состояние регистрации пользователя. `registered`Возможные значения: `enabled`,, `capable`и. `mfaRegistered` |

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