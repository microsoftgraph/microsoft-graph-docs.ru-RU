---
title: Тип ресурса Сигнинактивити
description: Предоставляет дату последнего входа для определенного пользователя.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e8300e787fe516a9712359f99ebf215f4813a0b9
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521231"
---
# <a name="signinactivity-resource-type"></a>Тип ресурса Сигнинактивити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет дату последнего входа для определенного [пользователя](user.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|ластсигниндатетиме|DateTimeOffset|Дата последнего входа для определенного пользователя. С помощью этого поля можно вычислить время последнего входа пользователя в каталог. Это поле можно использовать для создания отчетов, например неактивных пользователей. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Дополнительные сведения об использовании значения этого свойства содержатся [в разделе Manage неактивных учетных записей пользователей в Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).|
|ластсигнинрекуестид|String|Идентификатор запроса последнего входа, выполненного этим пользователем.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->