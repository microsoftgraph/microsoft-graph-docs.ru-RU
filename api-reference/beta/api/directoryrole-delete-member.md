---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2e5082488dbed8452abeecae904751ae3dff6dde
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436843"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="d8bad-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="d8bad-103">Remove directory role member</span></span>

<span data-ttu-id="d8bad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8bad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8bad-105">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="d8bad-105">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8bad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8bad-106">Permissions</span></span>

<span data-ttu-id="d8bad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8bad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d8bad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8bad-109">Permission type</span></span>      | <span data-ttu-id="d8bad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8bad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8bad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8bad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d8bad-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8bad-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d8bad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8bad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8bad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8bad-114">Not supported.</span></span>    |
|<span data-ttu-id="d8bad-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d8bad-115">Application</span></span> | <span data-ttu-id="d8bad-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="d8bad-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8bad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8bad-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d8bad-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8bad-118">Request headers</span></span>

| <span data-ttu-id="d8bad-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d8bad-119">Name</span></span>       | <span data-ttu-id="d8bad-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d8bad-120">Type</span></span> | <span data-ttu-id="d8bad-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d8bad-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d8bad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8bad-122">Authorization</span></span>  | <span data-ttu-id="d8bad-123">string</span><span class="sxs-lookup"><span data-stu-id="d8bad-123">string</span></span>  | <span data-ttu-id="d8bad-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8bad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8bad-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8bad-126">Request body</span></span>

<span data-ttu-id="d8bad-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8bad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8bad-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8bad-128">Response</span></span>

<span data-ttu-id="d8bad-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d8bad-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8bad-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d8bad-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8bad-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8bad-132">Request</span></span>

<span data-ttu-id="d8bad-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8bad-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8bad-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8bad-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryRoles/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="d8bad-135">C#</span><span class="sxs-lookup"><span data-stu-id="d8bad-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8bad-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8bad-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8bad-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8bad-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8bad-138">Java</span><span class="sxs-lookup"><span data-stu-id="d8bad-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8bad-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8bad-139">Response</span></span>

<span data-ttu-id="d8bad-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8bad-140">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


