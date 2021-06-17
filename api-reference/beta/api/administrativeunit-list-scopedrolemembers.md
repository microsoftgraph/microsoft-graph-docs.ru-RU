---
title: Список scopedRoleMembers
description: Извлечение списка ресурсов scopedRoleMembership.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 03dac66e6b3b20d34d9081f7b0a41d6111a4fdcf
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991976"
---
# <a name="list-scopedrolemembers"></a><span data-ttu-id="1d349-103">Список scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="1d349-103">List scopedRoleMembers</span></span>

<span data-ttu-id="1d349-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d349-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d349-105">Извлечение списка [ресурсов scopedRoleMembership.](../resources/scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="1d349-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) resources.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d349-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d349-106">Permissions</span></span>
<span data-ttu-id="1d349-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d349-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d349-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d349-109">Permission type</span></span>      | <span data-ttu-id="1d349-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d349-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d349-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d349-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1d349-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d349-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d349-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d349-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d349-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d349-114">Not supported.</span></span>    |
|<span data-ttu-id="1d349-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1d349-115">Application</span></span> | <span data-ttu-id="1d349-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d349-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d349-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d349-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1d349-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1d349-118">Optional query parameters</span></span>
<span data-ttu-id="1d349-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1d349-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d349-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d349-120">Request headers</span></span>
| <span data-ttu-id="1d349-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1d349-121">Name</span></span>      |<span data-ttu-id="1d349-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1d349-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d349-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d349-123">Authorization</span></span>  | <span data-ttu-id="1d349-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d349-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d349-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d349-126">Request body</span></span>
<span data-ttu-id="1d349-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d349-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d349-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d349-128">Response</span></span>

<span data-ttu-id="1d349-129">В случае успешного применения этот метод возвращает код ответа и коллекцию объектов `200 OK` [scopedRoleMembership](../resources/scopedrolemembership.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1d349-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d349-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1d349-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d349-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d349-131">Request</span></span>
<span data-ttu-id="1d349-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d349-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d349-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d349-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
```
# <a name="c"></a>[<span data-ttu-id="1d349-134">C#</span><span class="sxs-lookup"><span data-stu-id="1d349-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d349-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d349-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d349-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d349-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d349-137">Java</span><span class="sxs-lookup"><span data-stu-id="1d349-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1d349-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d349-138">Response</span></span>
<span data-ttu-id="1d349-p103">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1d349-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
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
  ]
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
