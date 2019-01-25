---
title: 'домен: forceDelete'
description: Удаление домена, с помощью асинхронной операции.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a1a2b2510f0c79f2be4e70deb9efabc65f8dfc4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527691"
---
# <a name="domain-forcedelete"></a>домен: forceDelete

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление домена, с помощью асинхронной операции.

В рамках этой операции выполняются следующие действия:

* Переименовывает имени участника-пользователя, EmailAddress и ProxyAddress пользователей с помощью ссылки на удаленный домен.

* Переименовывает EmailAddress групп ссылок на удаленный домен.

* Переименовывает identifierUris приложений с помощью ссылки на удаленный домен.

* Если число объектов, чтобы переименовать больше 1000, возвращается ошибка.

* Если один из приложений, чтобы переименовать приложения нескольких развертываний, возвращается ошибка.

После завершения удаления домена операции API для удаленного домена возвращает код ответа HTTP 404. Чтобы подтвердить удаление домена, можно выполнить [Получение домена](domain-get.md). Если домен был успешно удален, код ответа HTTP 404 будут возвращены в ответе.

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

| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный.|
| Content-Type  | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|disableUserAccounts|Логическое| Параметр, чтобы отключить переименованной учетных записей. Если учетная запись пользователя отключена, пользователь не разрешено вход.<br>*Значение true* (по умолчанию) — переименовано в рамках этой операции учетными записями пользователей.<br>*False* — переименовано в рамках этой операции учетные записи пользователей не отключены. |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `200 OK`. 

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

##### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
