---
title: Удаление oAuth2PermissionGrant
description: Удаление oAuth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: e594f6b0d46be47e80603bd5fdb3e259d85905f3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988967"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="685fb-103">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="685fb-103">Delete oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="685fb-104">Удаление oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="685fb-104">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="685fb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="685fb-105">Permissions</span></span>
<span data-ttu-id="685fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="685fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="685fb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="685fb-108">Permission type</span></span>      | <span data-ttu-id="685fb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="685fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="685fb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="685fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="685fb-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="685fb-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="685fb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="685fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="685fb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="685fb-113">Not supported.</span></span>    |
|<span data-ttu-id="685fb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="685fb-114">Application</span></span> | <span data-ttu-id="685fb-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="685fb-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="685fb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="685fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="685fb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="685fb-117">Request headers</span></span>
| <span data-ttu-id="685fb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="685fb-118">Name</span></span>       | <span data-ttu-id="685fb-119">Тип</span><span class="sxs-lookup"><span data-stu-id="685fb-119">Type</span></span> | <span data-ttu-id="685fb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="685fb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="685fb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="685fb-121">Authorization</span></span>  | <span data-ttu-id="685fb-122">string</span><span class="sxs-lookup"><span data-stu-id="685fb-122">string</span></span>  | <span data-ttu-id="685fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="685fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="685fb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="685fb-125">Request body</span></span>
<span data-ttu-id="685fb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="685fb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="685fb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="685fb-127">Response</span></span>

<span data-ttu-id="685fb-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="685fb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="685fb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="685fb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="685fb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="685fb-131">Request</span></span>
<span data-ttu-id="685fb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="685fb-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="685fb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="685fb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="685fb-134">C#</span><span class="sxs-lookup"><span data-stu-id="685fb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="685fb-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="685fb-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="685fb-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="685fb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="685fb-137">Java</span><span class="sxs-lookup"><span data-stu-id="685fb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="685fb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="685fb-138">Response</span></span>
<span data-ttu-id="685fb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="685fb-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
