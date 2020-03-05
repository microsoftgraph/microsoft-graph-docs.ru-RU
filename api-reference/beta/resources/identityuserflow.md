---
title: Тип ресурса Усерфлов
description: Пользовательские потоки идентификации — это встроенные пути проверки подлинности
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4fa3064d19d96a2a8297f72de6a625ee36c8db3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496553"
---
# <a name="userflow-resource-type"></a>Тип ресурса Усерфлов

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Потоки пользователей позволяют определить предопределенные настраиваемые политики для входа, регистрации, объединения и входа в систему, сброса пароля и обновления профиля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List](../api/identityuserflow-list.md) | Коллекция [усерфлов](identityuserflow.md) | Список Усерфловс. |
| [создание](../api/identityuserflow-post-userflows.md); | [усерфлов](identityuserflow.md) | Создание объекта Усерфлов. |
| [получение](../api/identityuserflow-get.md); | [усерфлов](identityuserflow.md) | Чтение свойств и связей объекта Усерфлов. |
| [удаление](../api/identityuserflow-delete.md); | Нет | Удаление объекта Усерфлов. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|усерфловтипе|строка| Возможные значения: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|усерфловтипеверсион|Одинарное| Это версия пользовательского типа. Каждый тип пользовательского типа может иметь различные варианты, например 1, 1,1 или 2.  |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "baseType": "",
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
