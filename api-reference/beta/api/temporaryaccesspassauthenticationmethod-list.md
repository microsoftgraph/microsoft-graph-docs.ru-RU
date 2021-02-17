---
title: Список temporaryAccessPassAuthenticationMethods
description: Получите список временных объектовAccessPassAuthenticationMethod и их свойств.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b44daae82d401da223d7012c662c9b3c9a97bec
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272706"
---
# <a name="list-temporaryaccesspassauthenticationmethods"></a>Список temporaryAccessPassAuthenticationMethods
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получить список временных [объектовAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  пользователя и их свойств. Этот вызов возвращает только один объект, так как для пользователей можно настроить только один метод временного доступа.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="permissions-acting-on-self"></a>Разрешения, действующие на себя

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

### <a name="permissions-acting-on-other-users"></a>Разрешения, действующие с другими пользователями

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|:-----------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All |


Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)

* Глобальный администратор
* Глобальный читатель
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод не поддерживает необязательные параметры запроса для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request"></a>Запрос 
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успеха этот метод возвращает код отклика и коллекцию временных `200 OK` [объектовAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в тексте отклика.  Этот вызов возвращает только один объект, так как для пользователей можно установить только один **временный объектAccessPassAuthenticationMethod.**

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/temporaryAccessPassMethods
```


### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.temporaryAccessPassAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
      "id": "String",
      "temporaryAccessPass": "String",
      "createdDateTime": "String (timestamp)",
      "startDateTime": "String (timestamp)",
      "lifetimeInMinutes": "Integer",
      "isUsableOnce": "Boolean",
      "isUsable": "Boolean",
      "methodUsabilityReason": "String"
    }
  ]
}
```
