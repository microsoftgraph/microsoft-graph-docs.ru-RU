---
title: Получение объекта appRoleAssignment
description: Получение свойств и связей объекта appRoleAssignment.
localization_priority: Priority
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1b9eded012eba7ed9cd2e0354698dc982f219ceb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945377"
---
# <a name="get-approleassignment"></a><span data-ttu-id="65b97-103">Получение объекта appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="65b97-103">Get appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65b97-104">Получение свойств и связей объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="65b97-104">Retrieve the properties and relationships of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="65b97-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65b97-105">Permissions</span></span>
<span data-ttu-id="65b97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65b97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65b97-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65b97-108">Permission type</span></span>      | <span data-ttu-id="65b97-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65b97-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65b97-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65b97-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65b97-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65b97-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65b97-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65b97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65b97-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65b97-113">Not supported.</span></span>    |
|<span data-ttu-id="65b97-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65b97-114">Application</span></span> | <span data-ttu-id="65b97-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65b97-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65b97-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65b97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignedTo
GET /groups/{id}/appRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65b97-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="65b97-117">Optional query parameters</span></span>
<span data-ttu-id="65b97-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="65b97-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65b97-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65b97-119">Request headers</span></span>
| <span data-ttu-id="65b97-120">Имя</span><span class="sxs-lookup"><span data-stu-id="65b97-120">Name</span></span>       | <span data-ttu-id="65b97-121">Тип</span><span class="sxs-lookup"><span data-stu-id="65b97-121">Type</span></span> | <span data-ttu-id="65b97-122">Описание</span><span class="sxs-lookup"><span data-stu-id="65b97-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65b97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65b97-123">Authorization</span></span>  | <span data-ttu-id="65b97-124">string</span><span class="sxs-lookup"><span data-stu-id="65b97-124">string</span></span>  | <span data-ttu-id="65b97-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65b97-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65b97-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65b97-127">Request body</span></span>
<span data-ttu-id="65b97-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65b97-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65b97-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="65b97-129">Response</span></span>

<span data-ttu-id="65b97-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [appRoleAssignment](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65b97-130">If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65b97-131">Пример</span><span class="sxs-lookup"><span data-stu-id="65b97-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65b97-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="65b97-132">Request</span></span>
<span data-ttu-id="65b97-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65b97-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="65b97-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="65b97-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65b97-135">C#</span><span class="sxs-lookup"><span data-stu-id="65b97-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65b97-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65b97-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65b97-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65b97-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65b97-138">Java</span><span class="sxs-lookup"><span data-stu-id="65b97-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="65b97-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="65b97-139">Response</span></span>
<span data-ttu-id="65b97-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65b97-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
