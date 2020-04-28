---
title: Удаление oAuth2PermissionGrant
description: Удаление oAuth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 14d70a5673ddf1e08f9aa50758befb85348efa1a
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199986"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="a563e-103">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a563e-103">Delete oAuth2PermissionGrant</span></span>

<span data-ttu-id="a563e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a563e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a563e-105">Удаление oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="a563e-105">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a563e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a563e-106">Permissions</span></span>
<span data-ttu-id="a563e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a563e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a563e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a563e-109">Permission type</span></span>      | <span data-ttu-id="a563e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a563e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a563e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a563e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a563e-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a563e-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a563e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a563e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a563e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a563e-114">Not supported.</span></span>    |
|<span data-ttu-id="a563e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a563e-115">Application</span></span> | <span data-ttu-id="a563e-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a563e-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a563e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a563e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a563e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a563e-118">Request headers</span></span>
| <span data-ttu-id="a563e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a563e-119">Name</span></span>       | <span data-ttu-id="a563e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a563e-120">Type</span></span> | <span data-ttu-id="a563e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a563e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a563e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a563e-122">Authorization</span></span>  | <span data-ttu-id="a563e-123">string</span><span class="sxs-lookup"><span data-stu-id="a563e-123">string</span></span>  | <span data-ttu-id="a563e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a563e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a563e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a563e-126">Request body</span></span>
<span data-ttu-id="a563e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a563e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a563e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a563e-128">Response</span></span>

<span data-ttu-id="a563e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a563e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a563e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a563e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a563e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a563e-132">Request</span></span>
<span data-ttu-id="a563e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a563e-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a563e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a563e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
# <a name="c"></a>[<span data-ttu-id="a563e-135">C#</span><span class="sxs-lookup"><span data-stu-id="a563e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a563e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a563e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a563e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a563e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a563e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a563e-138">Response</span></span>
<span data-ttu-id="a563e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a563e-139">Here is an example of the response.</span></span> 
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
