---
title: Тип ресурса UserFlow
description: Представляет поток пользователей удостоверений, включенный во встроенное путешествие по проверке подлинности.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4e03faaff265bf82bacf16a2db6c75e81176eafa
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883007"
---
# <a name="userflow-resource-type"></a>Тип ресурса UserFlow

Пространство имен: microsoft.graph

Потоки пользователей позволяют определить заранее настроенные политики для регистрации, регистрации, комбинированной регистрации и регистрации, сброса пароля и обновления профиля. Это базовый класс, который наследуют другие потоки пользователей.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Идентификатор потока пользователей. Префикс **B2C_1_** добавляется к предоставляемой вами стоимости.|
|userFlowType|userFlowType| Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Одинарное| Это версия типа потока пользователя. Каждый тип потока пользователей может иметь различные возможные версии, такие как 1, 1.1 или 2.  |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "userFlowType": "string",
  "userFlowTypeVersion": "Single"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UserFlow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
