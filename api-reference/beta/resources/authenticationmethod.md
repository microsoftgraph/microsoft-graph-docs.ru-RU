---
title: Тип ресурса authenticationMethod
description: Представляет метод проверки подлинности, зарегистрированный для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b9510a53ea80142bd9f155dce3e12824ad2d186e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034134"
---
# <a name="authenticationmethod-resource-type"></a>Тип ресурса authenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метод проверки подлинности, зарегистрированный для пользователя. [Способ проверки подлинности](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) используется пользователем для проверки подлинности или подтверждения удостоверения системы. В качестве примеров можно привести пароль, Телефон (с помощью SMS или голосового вызова), ключи безопасности FIDO2 и многое другое. В настоящее время применяются методы Password и Phone.

## <a name="methods"></a>Методы

| Метод       | Тип возвращаемых данных | Описание |
|:-------------|:------------|:------------|
| [Список Аусентикатионмесодс](../api/authentication-list-methods.md) | Коллекция [authenticationMethod](authenticationmethod.md) | Чтение свойств и связей всех объектов **authenticationMethod** пользователя. |
| [Получение параметра authenticationMethod](../api/authenticationmethod-get.md) | [Параметр authenticationmethod](authenticationmethod.md) | Чтение свойств и связей объекта **authenticationMethod** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Идентификатор этого экземпляра метода проверки подлинности, зарегистрированный для этого пользователя. Только для чтения. |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
  "baseType": "",
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


