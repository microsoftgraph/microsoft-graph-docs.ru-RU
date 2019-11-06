---
title: Обновление personName
description: Обновление свойств объекта PersonName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f288d73956b79c0ab5c47524239069f2c239791c
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997224"
---
# <a name="update-personname"></a>Обновление PersonName

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User. ReadWrite, User. ReadWrite. ALL          |
| Делегированные (личная учетная запись Майкрософт) | User. ReadWrite, User. ReadWrite. ALL          |
| Для приложений                            | User.ReadWrite.All                          |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/names/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           |Описание                  |
|:---------------|:----------------------------|
| Авторизация  | Bearer {токен}. Обязательный.   |
| Content-Type   | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип                                            | Описание                                                                             | 
|:-------------|:------------------------------------------------|:----------------------------------------------------------------------------------------|
|displayName   |Строка                                           | Предоставляет упорядоченную визуализацию имени и фамилии.                              |
|первыми         |String                                           | Имя пользователя.                                                                 |
|initials      |String                                           | Инициалы пользователя.                                                                   |
|лангуажетаг   |String                                           | Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.   |
|Фамили          |String                                           | Фамилия пользователя.                                                                  |
|маиден        |String                                           | Имя пользователя, марриаже фамилию.                                                          |
|назван        |String                                           | Отчество пользователя.                                                                     |
|прозвищ      |String                                           | Псевдоним пользователя.                                                                        |
|произношение |[йомиперсоннаме](../resources/yomipersonname.md) | Содержит сведения о произношении имени пользователя.                                 |
|суффикс        |String                                           | Обозначения, используемые после имени пользователя. (например, "доктор".)                                       |
|title         |String                                           | Хонорификс используется для префикса имени пользователя. (например, "доктор", "Sir", "Мадам", Mrs.)                      |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [PersonName](../resources/personname.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personname"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/names/{id}
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
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
HTTP/1.1 200 OK
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
  "description": "Update personname",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
