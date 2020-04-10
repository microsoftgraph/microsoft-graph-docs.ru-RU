---
title: Удаление Унифиедролеассигнмент
description: Удаление объекта Унифиедролеассигнмент.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93c7ee72c79b163b72aaa35b61277fd549a84cd5
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218999"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="f4c97-103">Удаление Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="f4c97-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="f4c97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4c97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4c97-105">Удаление объекта [унифиедролеассигнмент](../resources/unifiedRoleAssignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f4c97-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4c97-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4c97-106">Permissions</span></span>

<span data-ttu-id="f4c97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4c97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4c97-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4c97-109">Permission type</span></span>                        | <span data-ttu-id="f4c97-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4c97-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f4c97-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4c97-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4c97-112">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="f4c97-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="f4c97-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4c97-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4c97-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4c97-114">Not supported.</span></span> |
| <span data-ttu-id="f4c97-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4c97-115">Application</span></span>                            | <span data-ttu-id="f4c97-116">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="f4c97-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4c97-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4c97-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f4c97-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4c97-118">Request headers</span></span>

| <span data-ttu-id="f4c97-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f4c97-119">Name</span></span>          | <span data-ttu-id="f4c97-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f4c97-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f4c97-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4c97-121">Authorization</span></span> | <span data-ttu-id="f4c97-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f4c97-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4c97-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4c97-123">Request body</span></span>

<span data-ttu-id="f4c97-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4c97-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4c97-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4c97-125">Response</span></span>

<span data-ttu-id="f4c97-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f4c97-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4c97-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f4c97-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4c97-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4c97-129">Request</span></span>

<span data-ttu-id="f4c97-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4c97-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4c97-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4c97-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="f4c97-132">C#</span><span class="sxs-lookup"><span data-stu-id="f4c97-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4c97-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4c97-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4c97-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4c97-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4c97-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4c97-135">Response</span></span>

<span data-ttu-id="f4c97-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f4c97-136">The following is an example of the response.</span></span>

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
