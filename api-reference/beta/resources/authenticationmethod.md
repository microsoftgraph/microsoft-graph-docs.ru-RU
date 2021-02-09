---
title: Тип ресурса authenticationMethod
description: Представляет метод проверки подлинности, зарегистрированный для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f09780904d459ff628f9a13b21f3238611ede6ca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159159"
---
# <a name="authenticationmethod-resource-type"></a>Тип ресурса authenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метод проверки подлинности, зарегистрированный для пользователя. Метод [проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) используется пользователем для проверки подлинности или иной проверки подлинности в системе. Некоторые примеры включают пароль, телефон (можно использовать через SMS или голосовой вызов), ключи безопасности FIDO2 и другие.

## <a name="methods"></a>Методы

| Метод       | Тип возвращаемых данных | Описание |
|:-------------|:------------|:------------|
| [Список authenticationMethods](../api/authentication-list-methods.md) | [Коллекция authenticationMethod](authenticationmethod.md) | Чтение свойств и связей всех объектов **authenticationMethod** пользователя. |
| [Get authenticationMethod](../api/authenticationmethod-get.md) | [authenticationMethod](authenticationmethod.md) | Чтение свойств и связей объекта **authenticationMethod.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Идентификатор этого экземпляра метода проверки подлинности, зарегистрированного для этого пользователя. Только для чтения. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->