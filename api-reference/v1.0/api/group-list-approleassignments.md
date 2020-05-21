---
title: Список Аппролеассигнментс, назначенных группе
description: Получение списка Аппролеассигнментс, предоставленных группе.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 947271309c2e6aabc1dcce0760770eb3f2df7c12
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336550"
---
# <a name="list-approleassignments-granted-to-a-group"></a><span data-ttu-id="75eb4-103">Список Аппролеассигнментс, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="75eb4-103">List appRoleAssignments granted to a group</span></span>

<span data-ttu-id="75eb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75eb4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75eb4-105">Получение списка [аппролеассигнмент](../resources/approleassignment.md) , предоставленных группе.</span><span class="sxs-lookup"><span data-stu-id="75eb4-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="75eb4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75eb4-106">Permissions</span></span>

<span data-ttu-id="75eb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75eb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75eb4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75eb4-109">Permission type</span></span>      | <span data-ttu-id="75eb4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75eb4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75eb4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75eb4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="75eb4-112">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="75eb4-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="75eb4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75eb4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75eb4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75eb4-114">Not supported.</span></span>    |
|<span data-ttu-id="75eb4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75eb4-115">Application</span></span> | <span data-ttu-id="75eb4-116">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="75eb4-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75eb4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75eb4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75eb4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75eb4-118">Optional query parameters</span></span>

<span data-ttu-id="75eb4-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="75eb4-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75eb4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75eb4-120">Request headers</span></span>

| <span data-ttu-id="75eb4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="75eb4-121">Name</span></span>           | <span data-ttu-id="75eb4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="75eb4-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="75eb4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75eb4-123">Authorization</span></span>  | <span data-ttu-id="75eb4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75eb4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75eb4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75eb4-126">Request body</span></span>

<span data-ttu-id="75eb4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75eb4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75eb4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="75eb4-128">Response</span></span>

<span data-ttu-id="75eb4-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75eb4-129">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75eb4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="75eb4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="75eb4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="75eb4-131">Request</span></span>

<span data-ttu-id="75eb4-132">В приведенном ниже примере показан запрос на получение ролей приложения, назначенных группе.</span><span class="sxs-lookup"><span data-stu-id="75eb4-132">The following example shows a request to retrieve the app roles that have been assigned to a group.</span></span>


# <a name="http"></a>[<span data-ttu-id="75eb4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="75eb4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="75eb4-134">C#</span><span class="sxs-lookup"><span data-stu-id="75eb4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75eb4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75eb4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75eb4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75eb4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75eb4-137">Java</span><span class="sxs-lookup"><span data-stu-id="75eb4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75eb4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="75eb4-138">Response</span></span>

<span data-ttu-id="75eb4-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75eb4-139">The following is an example of the response.</span></span>

> <span data-ttu-id="75eb4-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75eb4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
