---
title: 'домен: forceDelete'
description: Удаляет домен с помощью асинхронной операции.
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d5e6d0a3e6334cee35790494e33f76e1dc2c2c43
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346172"
---
# <a name="domain-forcedelete"></a>домен: forceDelete

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаляет домен с помощью асинхронной операции.

Перед [вызовом forceDelete](domain-forcedelete.md) необходимо обновить или удалить ссылки на **Exchange в качестве** службы обеспечения.

В рамках этой операции выполняются следующие действия:

* Переименование upN, EmailAddress и ProxyAddress пользователей со ссылками на удаленный домен.

* Переименование emailAddress групп со ссылками на удаленный домен.

* Переименование идентификаторов приложений со ссылками на удаленный домен.

* Если число объектов, которые необходимо переименовать, превышает 1000, возвращается ошибка.

* Если одно из приложений, которое нужно переименовать, — это приложение с несколькими клиентами, возвращается ошибка.

После завершения удаления домена операции API для удаленного домена возвращают код ответа http 404. Чтобы проверить удаление домена, можно выполнить получить [домен](domain-get.md). Если домен был успешно удален, в ответе будет возвращен код ответа http 404.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Domain.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> В качестве параметра {id} укажите домен, используя его полное доменное имя.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {token}. Обязательный.|
| Content-Type  | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|disableUserAccounts|Логический| Параметр отключения переименованных учетных записей пользователей. Если учетная запись пользователя отключена, пользователю не будет разрешено войти.<br>*True* (по умолчанию) — учетные записи пользователей, переименованные в рамках этой операции, отключены.<br>*False* . Учетные записи пользователей, переименованные в рамках этой операции, не отключены. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK`. 

## <a name="example"></a>Пример
### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/domain-forcedelete-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/domain-forcedelete-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


