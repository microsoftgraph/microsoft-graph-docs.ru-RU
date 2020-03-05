---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f17f3fe1bb79a2d151e23bd4ee8172278e98b64d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434548"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="7ff82-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="7ff82-103">Remove directory role member</span></span>

<span data-ttu-id="7ff82-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7ff82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ff82-105">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="7ff82-105">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ff82-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff82-106">Permissions</span></span>

<span data-ttu-id="7ff82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ff82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ff82-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff82-109">Permission type</span></span>      | <span data-ttu-id="7ff82-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ff82-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ff82-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ff82-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7ff82-112">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="7ff82-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ff82-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ff82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ff82-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ff82-114">Not supported.</span></span>    |
|<span data-ttu-id="7ff82-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ff82-115">Application</span></span> | <span data-ttu-id="7ff82-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="7ff82-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ff82-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ff82-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7ff82-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ff82-118">Request headers</span></span>

| <span data-ttu-id="7ff82-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7ff82-119">Name</span></span>       | <span data-ttu-id="7ff82-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff82-120">Type</span></span> | <span data-ttu-id="7ff82-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff82-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ff82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ff82-122">Authorization</span></span>  | <span data-ttu-id="7ff82-123">string</span><span class="sxs-lookup"><span data-stu-id="7ff82-123">string</span></span>  | <span data-ttu-id="7ff82-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ff82-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ff82-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ff82-126">Request body</span></span>

<span data-ttu-id="7ff82-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ff82-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ff82-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ff82-128">Response</span></span>

<span data-ttu-id="7ff82-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7ff82-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ff82-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7ff82-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7ff82-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff82-132">Request</span></span>

<span data-ttu-id="7ff82-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ff82-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ff82-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff82-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="7ff82-135">C#</span><span class="sxs-lookup"><span data-stu-id="7ff82-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ff82-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ff82-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ff82-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ff82-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7ff82-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff82-138">Response</span></span>

<span data-ttu-id="7ff82-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ff82-139">Here is an example of the response.</span></span> 
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
