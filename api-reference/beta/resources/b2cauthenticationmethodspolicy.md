---
title: Тип ресурса b2cAuthenticationMethodsPolicy
description: Представляет метод проверки подлинности локальной учетной записи, зарегистрированный для пользователя, настроенного в клиенте Azure Active Directory (Azure AD) B2C.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74b18a2a0bc6d0ace2062f07d44eb175f7ad39e9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161763"
---
# <a name="b2cauthenticationmethodspolicy-resource-type"></a>Тип ресурса b2cAuthenticationMethodsPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) B2C позволяет администраторам клиента выбрать механизм разрешения конечным пользователям регистрироваться с помощью локальных учетных записей. Локальные учетные записи — это учетные записи, в которых утверждение удостоверения выполняется посредством Azure AD, а не поставщиком федеративных удостоверений, например Google или Facebook и т. д.

Локальные учетные записи в Azure AD B2C не используют параметры и парадигмы из Azure AD. Политика методов проверки подлинности Azure AD не используется и не внедряется службой Azure AD B2C. Azure AD B2C сохраняет эти параметры в другой политике, применяемой пользовательскими потоками.

## <a name="methods"></a>Методы

| Метод       | Тип возвращаемых данных | Описание |
|:-------------|:------------|:------------|
| [Получение b2cAuthenticationMethodsPolicy](../api/b2cauthenticationmethodspolicy-get.md) | [b2cauthenticationmethodspolicy](b2cauthenticationmethodspolicy.md) | Чтение свойств объекта **b2cauthenticationmethodspolicy**. |
| [Обновление b2cAuthenticationMethodsPolicy](../api/b2cauthenticationmethodspolicy-update.md) | Нет | Обновление свойств объекта **b2cauthenticationmethodspolicy**. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор политики методов проверки подлинности B2C. Это свойство только для чтения и ключ.|
|isEmailPasswordAuthenticationEnabled|Логическое|Администратор клиента может настраивать локальные учетные записи, используя электронную почту, если включен метод проверки подлинности электронной почты и пароля.|
|isUserNameAuthenticationEnabled|Логическое|Администратор клиента может настраивать локальные учетные записи, используя имя пользователя, если включен метод проверки подлинности электронной почты и пароля.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "b2cAuthenticationMethodsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
