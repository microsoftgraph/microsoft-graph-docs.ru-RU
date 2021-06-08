---
title: Принудительное удаление домена
description: Удаляет домен с помощью асинхронной длительной операции.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 50e5a418a40d9c5bedee1a007b491d15a06f3931
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787816"
---
# <a name="force-domain-deletion"></a>Принудительное удаление домена

Пространство имен: microsoft.graph

Удаляет домен с помощью асинхронной длительной операции.

Перед [вызовом forceDelete](domain-forcedelete.md)необходимо обновить или удалить ссылки на Exchange **в** качестве службы обеспечения.

В рамках этой операции выполняются следующие действия:

* Обновляет свойства и свойства домена со ссылками на удаленный домен для использования исходного onmicrosoft.com `userPrincipalName` `mail` `proxyAddresses` `users` домена.

* Обновляет свойство со ссылками на удаленный домен для использования исходного onmicrosoft.com `mail` `groups` домена.

* Обновляет свойство со ссылками на удаленный домен для использования исходного onmicrosoft.com `identifierUris` `applications` домена.

* Если число объектов, которые будут переименованы, превышает 1000, возвращается ошибка.

* Если одно из переименованных — это приложение с несколькими `applications` клиентами, возвращается ошибка.

После завершения удаления домена операции API для удаленного домена возвращают код состояния HTTP 404. Чтобы проверить удаление домена, можно выполнить операцию [получения домена.](domain-get.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Domain.ReadWrite.All |

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

## <a name="request-body"></a>Тело запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр | Тип | Описание |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| Параметр отключения учетных записей пользователей, которые переименованы. Если учетная запись пользователя отключена, пользователю не будет разрешено войти. Если **установлено,** что обновленная версия в рамках этой операции `users` будет отключена.  Значение по умолчанию: **true**. |

## <a name="response-body"></a>Текст отклика

В случае успешной работы этот метод возвращает `HTTP/1.1 204 OK` код состояния.

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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
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

