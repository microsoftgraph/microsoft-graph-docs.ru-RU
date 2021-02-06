---
title: Список объектов appRoleAssignment, предоставленных для пользователя
description: Получение списка назначений ролей приложений, предоставленных для пользователя.
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 6fa31fd31c8c898b508b9b0d02c602047eea58c5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136215"
---
# <a name="list-approleassignments-granted-to-a-user"></a><span data-ttu-id="4ea85-103">Список объектов appRoleAssignment, предоставленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="4ea85-103">List appRoleAssignments granted to a user</span></span>

<span data-ttu-id="4ea85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea85-105">Получение списка [appRoleAssignment](../resources/approleassignment.md), предоставленного пользователю.</span><span class="sxs-lookup"><span data-stu-id="4ea85-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that a user has been granted.</span></span> <span data-ttu-id="4ea85-106">Эта операция также возвращает роли приложений, назначенные группам, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="4ea85-106">This operation also returns app roles assigned to groups that the user is a direct member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ea85-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ea85-107">Permissions</span></span>

<span data-ttu-id="4ea85-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea85-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ea85-110">Permission type</span></span>      | <span data-ttu-id="4ea85-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ea85-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ea85-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ea85-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4ea85-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ea85-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="4ea85-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ea85-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ea85-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ea85-115">Not supported.</span></span>    |
|<span data-ttu-id="4ea85-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ea85-116">Application</span></span> | <span data-ttu-id="4ea85-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea85-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ea85-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ea85-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ea85-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ea85-119">Optional query parameters</span></span>

<span data-ttu-id="4ea85-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4ea85-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ea85-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ea85-121">Request headers</span></span>

| <span data-ttu-id="4ea85-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4ea85-122">Name</span></span>           | <span data-ttu-id="4ea85-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea85-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="4ea85-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ea85-124">Authorization</span></span>  | <span data-ttu-id="4ea85-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ea85-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ea85-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ea85-127">Request body</span></span>

<span data-ttu-id="4ea85-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ea85-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ea85-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ea85-129">Response</span></span>

<span data-ttu-id="4ea85-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [appRoleAssignment](../resources/approleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4ea85-130">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ea85-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4ea85-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ea85-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ea85-132">Request</span></span>

<span data-ttu-id="4ea85-133">В приведенном примере показано, как запросить извлечение ролей приложения, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="4ea85-133">Here is an example of the request to retrieve the app roles that have been assigned to a user.</span></span>


# <a name="http"></a>[<span data-ttu-id="4ea85-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea85-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="4ea85-135">C#</span><span class="sxs-lookup"><span data-stu-id="4ea85-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ea85-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ea85-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ea85-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ea85-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ea85-138">Java</span><span class="sxs-lookup"><span data-stu-id="4ea85-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4ea85-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ea85-139">Response</span></span>

<span data-ttu-id="4ea85-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ea85-140">The following is an example of the response.</span></span> 

> <span data-ttu-id="4ea85-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ea85-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


