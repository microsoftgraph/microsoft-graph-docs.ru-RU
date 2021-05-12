---
title: тип ресурса authenticationMethod
description: Представляет метод проверки подлинности, зарегистрированный пользователем.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9ab808934491793b796be1c66fc87051ed6e9b29
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335627"
---
# <a name="authenticationmethod-resource-type"></a>тип ресурса authenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метод проверки подлинности, зарегистрированный пользователем. Метод [проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) — это то, что используется пользователем для проверки подлинности или иного доказательства его подлинности в системе. Некоторые примеры включают пароль, телефон (можно использовать SMS или голосовой вызов), ключи безопасности FIDO2 и другие.

> [!IMPORTANT]
> Перечисление методов проверки подлинности пользователей возвращает только методы, поддерживаемые в этой версии API. Обзор [API методов проверки подлинности Azure AD](authenticationmethods-overview.md) см. в списке поддерживаемых в настоящее время методов.

## <a name="methods"></a>Методы

| Метод       | Тип возвращаемых данных | Описание |
|:-------------|:------------|:------------|
| [Проверка подлинности спискаМетходы](../api/authentication-list-methods.md) | [коллекция authenticationMethod](authenticationmethod.md) | Ознакомьтесь с свойствами и отношениями всех объектов проверки подлинности **пользователяMethod.** |

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