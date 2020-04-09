---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0cf8a6f58439a6bcd7c6605503b8c4d471d9f188
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181429"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="a1197-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="a1197-103">Remove directory role member</span></span>

<span data-ttu-id="a1197-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1197-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1197-105">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="a1197-105">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1197-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1197-106">Permissions</span></span>

<span data-ttu-id="a1197-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a1197-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1197-109">Permission type</span></span>      | <span data-ttu-id="a1197-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1197-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1197-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1197-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a1197-112">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="a1197-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a1197-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1197-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1197-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1197-114">Not supported.</span></span>    |
|<span data-ttu-id="a1197-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1197-115">Application</span></span> | <span data-ttu-id="a1197-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a1197-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1197-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1197-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a1197-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1197-118">Request headers</span></span>

| <span data-ttu-id="a1197-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a1197-119">Name</span></span>       | <span data-ttu-id="a1197-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a1197-120">Type</span></span> | <span data-ttu-id="a1197-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a1197-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1197-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1197-122">Authorization</span></span>  | <span data-ttu-id="a1197-123">string</span><span class="sxs-lookup"><span data-stu-id="a1197-123">string</span></span>  | <span data-ttu-id="a1197-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1197-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1197-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1197-126">Request body</span></span>

<span data-ttu-id="a1197-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1197-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1197-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1197-128">Response</span></span>

<span data-ttu-id="a1197-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a1197-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1197-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a1197-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a1197-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1197-132">Request</span></span>

<span data-ttu-id="a1197-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1197-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1197-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1197-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="a1197-135">C#</span><span class="sxs-lookup"><span data-stu-id="a1197-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1197-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1197-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1197-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1197-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1197-138">Java</span><span class="sxs-lookup"><span data-stu-id="a1197-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a1197-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1197-139">Response</span></span>

<span data-ttu-id="a1197-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1197-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
