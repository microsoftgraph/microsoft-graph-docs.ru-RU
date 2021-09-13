---
title: Тип ресурса UserFlow
description: Представляет поток пользователей удостоверений, включенный во встроенное путешествие по проверке подлинности.
ms.localizationpriority: medium
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f2cf68cf056f694c33052e23f9c78db2573c3424
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067362"
---
# <a name="userflow-resource-type"></a>Тип ресурса UserFlow

Пространство имен: microsoft.graph

Потоки пользователей позволяют определить заранее настроенные политики для регистрации, регистрации, комбинированной регистрации и регистрации, сброса пароля и обновления профиля. Это базовый класс, который наследуют другие потоки пользователей.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Идентификатор потока пользователей. Префикс **B2C_1_** добавляется к предоставляемой вами стоимости.|
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
