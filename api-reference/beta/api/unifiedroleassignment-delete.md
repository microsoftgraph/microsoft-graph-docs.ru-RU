---
title: Удаление Унифиедролеассигнмент
description: Удаление объекта Унифиедролеассигнмент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3d8e55560e01c7c63613566e375d8c03b9b36230
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461854"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="0a9f8-103">Удаление Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="0a9f8-103">Delete unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a9f8-104">Удаление объекта [унифиедролеассигнмент](../resources/unifiedRoleAssignment.md) .</span><span class="sxs-lookup"><span data-stu-id="0a9f8-104">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a9f8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a9f8-105">Permissions</span></span>

<span data-ttu-id="0a9f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a9f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a9f8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a9f8-108">Permission type</span></span>                        | <span data-ttu-id="0a9f8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a9f8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0a9f8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a9f8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a9f8-111">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="0a9f8-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="0a9f8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a9f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a9f8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a9f8-113">Not supported.</span></span> |
| <span data-ttu-id="0a9f8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a9f8-114">Application</span></span>                            | <span data-ttu-id="0a9f8-115">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="0a9f8-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a9f8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a9f8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0a9f8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a9f8-117">Request headers</span></span>

| <span data-ttu-id="0a9f8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0a9f8-118">Name</span></span>          | <span data-ttu-id="0a9f8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0a9f8-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0a9f8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a9f8-120">Authorization</span></span> | <span data-ttu-id="0a9f8-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0a9f8-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a9f8-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a9f8-122">Request body</span></span>

<span data-ttu-id="0a9f8-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a9f8-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a9f8-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a9f8-124">Response</span></span>

<span data-ttu-id="0a9f8-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0a9f8-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a9f8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0a9f8-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a9f8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a9f8-128">Request</span></span>

<span data-ttu-id="0a9f8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a9f8-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a9f8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a9f8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a9f8-131">C#</span><span class="sxs-lookup"><span data-stu-id="0a9f8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a9f8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a9f8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a9f8-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0a9f8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a9f8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a9f8-134">Response</span></span>

<span data-ttu-id="0a9f8-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0a9f8-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
