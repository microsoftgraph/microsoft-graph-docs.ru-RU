---
title: Get a scopedRoleMember
description: Извлечение определенного ресурса scopedRoleMembership.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0f63cb587d3751a81482e5ce2c6ed3f05f2dc5c3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943021"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="e25ce-103">Get a scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="e25ce-103">Get a scopedRoleMember</span></span>

<span data-ttu-id="e25ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e25ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e25ce-105">Извлечение [определенного ресурса scopedRoleMembership.](../resources/scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="e25ce-105">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="e25ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e25ce-106">Permissions</span></span>
<span data-ttu-id="e25ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e25ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e25ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e25ce-109">Permission type</span></span>      | <span data-ttu-id="e25ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e25ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e25ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e25ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e25ce-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e25ce-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e25ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e25ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e25ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e25ce-114">Not supported.</span></span>    |
|<span data-ttu-id="e25ce-115">Application</span><span class="sxs-lookup"><span data-stu-id="e25ce-115">Application</span></span> | <span data-ttu-id="e25ce-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e25ce-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e25ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e25ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e25ce-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e25ce-118">Optional query parameters</span></span>
<span data-ttu-id="e25ce-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e25ce-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e25ce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e25ce-120">Request headers</span></span>
| <span data-ttu-id="e25ce-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e25ce-121">Name</span></span>      |<span data-ttu-id="e25ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e25ce-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e25ce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e25ce-123">Authorization</span></span>  | <span data-ttu-id="e25ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e25ce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e25ce-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e25ce-126">Request body</span></span>
<span data-ttu-id="e25ce-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e25ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e25ce-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e25ce-128">Response</span></span>

<span data-ttu-id="e25ce-129">В случае успешного применения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [scopedRoleMembership](../resources/scopedrolemembership.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e25ce-129">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e25ce-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e25ce-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e25ce-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e25ce-131">Request</span></span>
<span data-ttu-id="e25ce-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e25ce-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e25ce-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e25ce-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="e25ce-134">C#</span><span class="sxs-lookup"><span data-stu-id="e25ce-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e25ce-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e25ce-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e25ce-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e25ce-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e25ce-137">Java</span><span class="sxs-lookup"><span data-stu-id="e25ce-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e25ce-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e25ce-138">Response</span></span>
<span data-ttu-id="e25ce-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e25ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
