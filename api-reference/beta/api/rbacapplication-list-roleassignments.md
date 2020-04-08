---
title: Список Унифиедролеассигнментс
description: Получение списка объектов Унифиедролеассигнмент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b8117c54cb571a3cb3dcf43699e1356459f13220
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181205"
---
# <a name="list-unifiedroleassignments"></a>Список Унифиедролеассигнментс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [унифиедролеассигнмент](../resources/unifiedroleassignment.md) для поставщика.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Для `$filter` выполнения этой операции требуется параметр запроса. Вы можете отфильтровать `roleDefinitionId` по `principalId` свойствам или. `roleDefinitionId` Свойство может быть идентификатором объекта Role или шаблоном роли. Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Authorization | Bearer {token} |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-request-using-a-filter-on-role-definition-id"></a>Пример 1: запрос с использованием фильтра по ИДЕНТИФИКАТОРу определения роли

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGnbHktRMANMpnGtLZ3MXeY-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "4b1edb69-3051-4c03-a671-ad2d9dcc5de6",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEKLh1vKaL9NIi6cTuyyN_6Q-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "f2d6e1a2-2f9a-48d3-8ba7-13bb2c8dffa4",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGXxIcn3O7hBqaGB0NGuCwE-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "c921f165-3bf7-41b8-a9a1-81d0d1ae0b01",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEAWO6-FSXqhEg1mkkLETmA8-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "e1eb8e05-5e52-44a8-8359-a490b113980f",
            "directoryScopeId": "/"
        }
    ]
}
```

### <a name="example-2-request-using-a-filter-on-principal-id"></a>Пример 2: запрос с использованием фильтра по ИДЕНТИФИКАТОРу субъекта

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=principalId eq 'a98eb769-7bd4-4489-86f6-ad96e1d58b62'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "uBph6InB6EaU4WAhOrH4FGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "e8611ab8-c189-46e8-94e1-60213ab1f814",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "5wuT_mJe20eRr5jDpJo4sWm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "5TgczyE2BECny4eWJNztfGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "cf1c38e5-3621-4004-a7cb-879624dced7c",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "CRCUdVqRaUir52kb_xgnnmm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "75941009-915a-4869-abe7-691bff18279e",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "4yeYchSc90m7G5YI8Va7uGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "y-RKGSaxskC9W2CRs4CXfWm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
