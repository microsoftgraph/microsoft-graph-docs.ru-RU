---
title: Список scopedMembers для роли каталога
description: Извлечение списка объектов scopedRoleMembership для роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d5f915debcdecba1effdf96bae6ae36da0331783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207745"
---
# <a name="list-scopedmembers-for-a-directory-role"></a>Список scopedMembers для роли каталога

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка [объектов scopedRoleMembership](../resources/scopedrolemembership.md) для роли каталога.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{role-id}/scopedMembers
GET /directoryroles/roleTemplateId={roleTemplateId}/scopedMembers
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного применения этот метод возвращает код ответа и коллекцию объектов `200 OK` [scopedRoleMembership](../resources/scopedrolemembership.md) в тексте ответа.
## <a name="examples"></a>Примеры

### <a name="example-1--get-the-scoped-members-of-a-directory-role-using-role-id"></a>Пример 1. Получить масштабные члены роли каталога с помощью role id

#### <a name="request"></a>Запрос
Ниже приводится пример запроса на id роли **каталога** `41d12a2f-caa8-4e3e-ba14-05e5102ce085` .

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/41d12a2f-caa8-4e3e-ba14-05e5102ce085/scopedMembers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
Ниже показан пример отклика. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
            }
        }
    ]
}
```

### <a name="example-2--get-the-scoped-members-of-a-directory-role-using-roletemplateid"></a>Пример 2. Получить масштабные члены роли каталога с помощью roleTemplateId

#### <a name="request"></a>Запрос
Ниже приводится пример запроса на роль каталога с **roleTemplateId** `fdd7a751-b60b-444a-984c-02652fe8fa1c` .


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c/scopedMembers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже показан пример отклика. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
