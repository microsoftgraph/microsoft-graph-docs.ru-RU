---
title: Принудительное удаление домена
description: Удаляет домен с помощью асинхронной длительной операции.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9219a6e49cc0c0ddc223ea1d9dd108903a21cd0
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228833"
---
# <a name="force-domain-deletion"></a>Принудительное удаление домена

Пространство имен: microsoft.graph

Удаляет домен с помощью асинхронной длительной операции.

В рамках этой операции выполняются следующие действия:

* Обновляет свойства `userPrincipalName`, `mail`и `proxyAddresses` свойства `users` со ссылками на удаленный домен, чтобы использовать исходный домен onmicrosoft.com.

* Обновляет `mail` свойство `groups` со ссылками на удаленный домен, чтобы использовать исходный домен onmicrosoft.com.

* Обновляет `identifierUris` свойство `applications` со ссылками на удаленный домен, чтобы использовать исходный домен onmicrosoft.com.

* Если количество переименованных объектов больше 1000, возвращается ошибка.

* Если одно из `applications` наименования является приложением с несколькими клиентами, возвращается ошибка.

После завершения удаления домена операции API для удаленного домена будут возвращать код состояния HTTP 404. Чтобы проверить удаление домена, можно выполнить операцию [получения домена](domain-get.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> В качестве параметра {id} укажите домен, используя его полное доменное имя.

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный.|
| Content-Type  | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр | Тип | Описание |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| Параметр для отключения переименованных учетных записей пользователей. Если учетная запись пользователя отключена, пользователь не может войти в систему. Если задано **значение true** , то `users` обновление в рамках этой операции будет отключено.  Значение по умолчанию: **true**. |

## <a name="response-body"></a>Текст ответа

В случае успеха этот метод возвращает `HTTP/1.1 204 OK` код состояния.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/v1.0/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
