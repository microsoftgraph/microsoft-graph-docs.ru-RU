---
title: Get a scopedRoleMember
description: Извлечение определенного ресурса scopedRoleMembership.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f533f0fffbcc95e52795d2c8d51eb52ba610f3a0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433042"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="f9edb-103">Get a scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="f9edb-103">Get a scopedRoleMember</span></span>

<span data-ttu-id="f9edb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9edb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9edb-105">Извлечение [определенного ресурса scopedRoleMembership.](../resources/scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="f9edb-105">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9edb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9edb-106">Permissions</span></span>
<span data-ttu-id="f9edb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9edb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f9edb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9edb-109">Permission type</span></span>      | <span data-ttu-id="f9edb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9edb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9edb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9edb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9edb-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9edb-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f9edb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9edb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9edb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9edb-114">Not supported.</span></span>    |
|<span data-ttu-id="f9edb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9edb-115">Application</span></span> | <span data-ttu-id="f9edb-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9edb-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9edb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9edb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9edb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9edb-118">Optional query parameters</span></span>
<span data-ttu-id="f9edb-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9edb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9edb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9edb-120">Request headers</span></span>
| <span data-ttu-id="f9edb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f9edb-121">Name</span></span>      |<span data-ttu-id="f9edb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f9edb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9edb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9edb-123">Authorization</span></span>  | <span data-ttu-id="f9edb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9edb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9edb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9edb-126">Request body</span></span>
<span data-ttu-id="f9edb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9edb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9edb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9edb-128">Response</span></span>

<span data-ttu-id="f9edb-129">В случае успешного применения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [scopedRoleMembership](../resources/scopedrolemembership.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f9edb-129">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9edb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f9edb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9edb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9edb-131">Request</span></span>
<span data-ttu-id="f9edb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9edb-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f9edb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9edb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="f9edb-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9edb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9edb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9edb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9edb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9edb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9edb-137">Java</span><span class="sxs-lookup"><span data-stu-id="f9edb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="f9edb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9edb-138">Response</span></span>
<span data-ttu-id="f9edb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9edb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
