---
author: swapnil1993
title: Удаление contentType
description: Удаление типа контента из SharePoint или сайта.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 9597f4b66a070ee40199b39f8accc8b3ab9f5c0e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439412"
---
# <a name="delete-contenttype"></a><span data-ttu-id="bc106-103">Удаление contentType</span><span class="sxs-lookup"><span data-stu-id="bc106-103">Delete contentType</span></span>
<span data-ttu-id="bc106-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc106-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc106-105">Удаление [типа контента][contentType] из [списка][] или [сайта.][]</span><span class="sxs-lookup"><span data-stu-id="bc106-105">Remove a [content type][contentType] from a [list][] or a [site][].</span></span>


## <a name="permissions"></a><span data-ttu-id="bc106-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc106-106">Permissions</span></span>
<span data-ttu-id="bc106-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc106-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="bc106-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc106-109">Permission type</span></span>      | <span data-ttu-id="bc106-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc106-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc106-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc106-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc106-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bc106-112">Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="bc106-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc106-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc106-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc106-114">Not supported.</span></span>    |
|<span data-ttu-id="bc106-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="bc106-115">Application</span></span> | <span data-ttu-id="bc106-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bc106-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc106-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc106-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a><span data-ttu-id="bc106-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc106-118">Request headers</span></span>
|<span data-ttu-id="bc106-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bc106-119">Name</span></span>|<span data-ttu-id="bc106-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bc106-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bc106-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc106-121">Authorization</span></span>|<span data-ttu-id="bc106-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc106-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="bc106-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc106-124">Request body</span></span>

<span data-ttu-id="bc106-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc106-125">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc106-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc106-126">Response</span></span>

<span data-ttu-id="bc106-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bc106-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bc106-128">Пример</span><span class="sxs-lookup"><span data-stu-id="bc106-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc106-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc106-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bc106-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc106-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
```
# <a name="c"></a>[<span data-ttu-id="bc106-131">C#</span><span class="sxs-lookup"><span data-stu-id="bc106-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc106-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc106-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc106-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc106-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc106-134">Java</span><span class="sxs-lookup"><span data-stu-id="bc106-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bc106-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc106-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
