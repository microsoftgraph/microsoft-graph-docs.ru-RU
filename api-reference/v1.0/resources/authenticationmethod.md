---
title: тип ресурса authenticationMethod
description: Представляет метод проверки подлинности, зарегистрированный пользователем.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 92c504bf5cbbec90c11bb51c6d8e19a67e4d7cfb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127047"
---
# <a name="authenticationmethod-resource-type"></a>тип ресурса authenticationMethod

Пространство имен: microsoft.graph

Представляет метод проверки подлинности, зарегистрированный пользователем. Метод [проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) — это то, что используется пользователем для проверки подлинности или иного доказательства его подлинности в системе. Некоторые примеры включают пароль, телефон (можно использовать с помощью SMS или голосового звонка), ключи безопасности FIDO2 и другие.

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

## <a name="relationships"></a>Отношения

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
