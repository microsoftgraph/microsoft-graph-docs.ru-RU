---
title: Предоставление Аппролеассигнмент участнику службы
description: Предоставьте участнику службы назначение роли приложения.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 8b99ea2f6f5513c6673a226ef13616785e9dea98
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335889"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a>Предоставление Аппролеассигнмент участнику службы

Пространство имен: microsoft.graph


Назначьте роль приложения участнику клиентской службы.

Роли приложений, назначенные субъектам служб, также называются [разрешениями приложений](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types). Разрешения приложения могут быть предоставлены непосредственно с назначениями ролей приложения или с помощью [согласия пользователя](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).

Чтобы назначить роль приложения для участника клиентской службы, необходимы три идентификатора:

- `principalId`: `id` Клиент службы, которому назначается роль приложения.
- `resourceId`: `id` Ресурс `servicePrincipal` (API), в котором определена роль приложения (разрешение приложения).
- `appRoleId`: Значение `id` `appRole` (заданное для субъекта-службы ресурса), которое необходимо назначить участнику клиентской службы.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Аппролеассигнмент. ReadWrite. ALL, |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> Рекомендуется создавать назначения ролей приложений с помощью [ `appRoleAssignedTo` отношения между субъектом службы _ресурсов_ ](serviceprincipal-post-approleassignedto.md), а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:----------|
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Основной текст запроса

В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В этом примере и то, `{id}` и другое — это `{principalId-value}` `id` назначенный субъект-службу клиента, и будет `{resoruceId}` иметь значение `id` субъекта-службы ресурсов (API).

### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "id": "id-value",
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalType": "principalType-value",
  "principalId": "principalId-value",
  "principalDisplayName": "principalDisplayName-value",
  "resourceId": "resourceId-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
