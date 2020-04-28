---
title: Создание personName
description: Используйте этот API, чтобы создать новый personName в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: dd9b66db16f3c9146b47e917d9417ac7bb7e7adb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455094"
---
# <a name="create-personname"></a>Создание personName

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот API, чтобы создать новый объект [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL |
| Для приложений                            | User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           |Описание                  |
|:---------------|:----------------------------|
| Авторизация  | Bearer {токен}. Обязательный.   |
| Content-Type   | application/json. Обязательный. |

## <a name="request-body"></a>Основной текст запроса

В тексте запроса добавьте представление объекта [PersonName](../resources/personname.md) в формате JSON.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [PersonName](../resources/personname.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
