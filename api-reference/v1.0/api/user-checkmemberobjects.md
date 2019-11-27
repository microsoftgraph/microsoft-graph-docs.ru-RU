---
title: 'Пользователь: Чеккмемберобжектс'
description: Проверка членства в списке ролей группы или каталога для указанного объекта пользователя.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da8993fb65fcc9a0a7bb0f887c3e743b196c686a
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621637"
---
# <a name="user-checkmemberobjects"></a>Пользователь: Чеккмемберобжектс

Проверка членства в списке ролей группы или каталога для указанного объекта пользователя. Этот метод является транзитивным.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User. ReadBasic, User. Read. ALL, User. ReadWrite. ALL<br><br>Дополнительно:<br><br><ul><li>Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</li><li>При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</li><li>Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</li></ul>Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All  |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL<br>С<ul><li>Если выполняется проверка членства в группах: Group. Read. ALL, Group. ReadWrite. ALL</li><li>При проверке принадлежности к административным единицам: AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</li><li>Если выполняется проверка членства в ролях каталога: Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</li></ul>Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|ids|Коллекция String|Коллекция, содержащая идентификаторы объектов групп, ролей каталогов или идентификаторов Ролетемплате для ролей каталогов, в которых проверяется членство. Можно указать до 20 объектов.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции String в тексте отклика.

## <a name="examples"></a>Примеры

Ниже приведен пример вызова этого API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
