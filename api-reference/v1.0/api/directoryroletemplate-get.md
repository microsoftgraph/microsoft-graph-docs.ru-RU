---
title: Вывод объекта directoryRoleTemplate
description: Получение свойств и связей объекта directoryRoleTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45d6981b8c89bb061086045094ce8f5bc22c8671
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016715"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="06d3f-103">Вывод объекта directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="06d3f-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="06d3f-104">Получение свойств и связей объекта directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="06d3f-104">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="06d3f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06d3f-105">Permissions</span></span>
<span data-ttu-id="06d3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06d3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06d3f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06d3f-108">Permission type</span></span>      | <span data-ttu-id="06d3f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06d3f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06d3f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06d3f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06d3f-111">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="06d3f-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06d3f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06d3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06d3f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d3f-113">Not supported.</span></span>    |
|<span data-ttu-id="06d3f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06d3f-114">Application</span></span> | <span data-ttu-id="06d3f-115">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="06d3f-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06d3f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06d3f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="06d3f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06d3f-117">Optional query parameters</span></span>
<span data-ttu-id="06d3f-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="06d3f-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="06d3f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06d3f-119">Request headers</span></span>
| <span data-ttu-id="06d3f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="06d3f-120">Name</span></span>       | <span data-ttu-id="06d3f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="06d3f-121">Type</span></span> | <span data-ttu-id="06d3f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="06d3f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06d3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06d3f-123">Authorization</span></span>  | <span data-ttu-id="06d3f-124">string</span><span class="sxs-lookup"><span data-stu-id="06d3f-124">string</span></span>  | <span data-ttu-id="06d3f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06d3f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06d3f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06d3f-127">Request body</span></span>
<span data-ttu-id="06d3f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06d3f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06d3f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d3f-129">Response</span></span>

<span data-ttu-id="06d3f-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="06d3f-130">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06d3f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="06d3f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06d3f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d3f-132">Request</span></span>
<span data-ttu-id="06d3f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06d3f-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="06d3f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="06d3f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06d3f-135">C#</span><span class="sxs-lookup"><span data-stu-id="06d3f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06d3f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="06d3f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06d3f-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="06d3f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="06d3f-138">Java</span><span class="sxs-lookup"><span data-stu-id="06d3f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="06d3f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d3f-139">Response</span></span>
<span data-ttu-id="06d3f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06d3f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
