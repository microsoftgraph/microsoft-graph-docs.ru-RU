---
title: Создание externalGroupMember
description: Создание нового внешнего объектаGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d08e2646d34a165ac49176a1694613bd735682d4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956051"
---
# <a name="create-externalgroupmember"></a>Создание externalGroupMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [внешнего объектаGroupMember.](../resources/externalgroupmember.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Не поддерживается                               |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Приложение                            | ExternalItem.ReadWrite.All                  |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON внешнего [объектаGroupMember.](../resources/externalgroupmember.md)

В следующей таблице показаны свойства, необходимые при создании [externalGroupMember.](../resources/externalgroupmember.md)

| Свойство       | Тип                    | Описание                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| id             | Строка                  | Уникальный `id` член. Это будет objectId в случае пользователей Или групп Azure Active Directory и externalGroupId в случае внешних групп.                                    |
| type           | externalGroupMemberType | Тип участника, добавленного во внешнюю группу. Возможные значения: или когда identitySource является и только `user` `group` `azureActiveDirectory` `group` тогда, когда identitySource `external` является . |
| identitySource | identitySourceType      | Источник удостоверений, к которой принадлежит член. Возможные значения: `azureActiveDirectory`, `external`.                                                                                         |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [внешний объектGroupMember](../resources/externalgroupmember.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a>Пример 1. Добавление пользователя Azure Active Directory в качестве участника

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a>Пример 2. Добавление группы Azure Active Directory в качестве участника

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a>Пример 3. Добавление другой внешней группы в качестве участника

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from__3"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "1431b9c38ee647f6a",
  "type": "group",
  "identitySource": "external"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "14m1b9c38qe647f6a",
  "type": "group",
  "identitySource": "external"
}
```
