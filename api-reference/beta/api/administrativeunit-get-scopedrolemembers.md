---
title: Получение Скопедролемембер
description: Получение определенного ресурса Scopedrolemembership изменен.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7357cf52388b2abdd72e81691ea70f8da77f7b4f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408729"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="bfcd7-103">Получение Скопедролемембер</span><span class="sxs-lookup"><span data-stu-id="bfcd7-103">Get a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfcd7-104">Получение определенного ресурса [scopedrolemembership изменен](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="bfcd7-104">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfcd7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfcd7-105">Permissions</span></span>
<span data-ttu-id="bfcd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfcd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bfcd7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfcd7-108">Permission type</span></span>      | <span data-ttu-id="bfcd7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfcd7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfcd7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfcd7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bfcd7-111">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="bfcd7-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bfcd7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfcd7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfcd7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfcd7-113">Not supported.</span></span>    |
|<span data-ttu-id="bfcd7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfcd7-114">Application</span></span> | <span data-ttu-id="bfcd7-115">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bfcd7-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfcd7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfcd7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfcd7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bfcd7-117">Optional query parameters</span></span>
<span data-ttu-id="bfcd7-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bfcd7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfcd7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfcd7-119">Request headers</span></span>
| <span data-ttu-id="bfcd7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bfcd7-120">Name</span></span>      |<span data-ttu-id="bfcd7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bfcd7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bfcd7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfcd7-122">Authorization</span></span>  | <span data-ttu-id="bfcd7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfcd7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfcd7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bfcd7-125">Request body</span></span>
<span data-ttu-id="bfcd7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfcd7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfcd7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfcd7-127">Response</span></span>

<span data-ttu-id="bfcd7-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bfcd7-128">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfcd7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bfcd7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfcd7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfcd7-130">Request</span></span>
<span data-ttu-id="bfcd7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfcd7-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bfcd7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfcd7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bfcd7-133">C#</span><span class="sxs-lookup"><span data-stu-id="bfcd7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfcd7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfcd7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bfcd7-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bfcd7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bfcd7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfcd7-136">Response</span></span>
<span data-ttu-id="bfcd7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfcd7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
