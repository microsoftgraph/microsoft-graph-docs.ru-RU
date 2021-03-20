---
author: swapnil1993
title: Удаление columnDefinition
description: Удаление столбца с сайта, списка или типа контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 771123af410d5c0c63038f6d032e5c56874d058f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952334"
---
# <a name="delete-columndefinition"></a><span data-ttu-id="b40bf-103">Удаление columnDefinition</span><span class="sxs-lookup"><span data-stu-id="b40bf-103">Delete columnDefinition</span></span>
<span data-ttu-id="b40bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b40bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="b40bf-105">Удаление [столбца][columndefinition] с [сайта,][] [списка или][] [типа контента.][contentType]</span><span class="sxs-lookup"><span data-stu-id="b40bf-105">Remove a [column][columndefinition] from a [site][], [list][] or [content type][contentType].</span></span>


## <a name="permissions"></a><span data-ttu-id="b40bf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b40bf-106">Permissions</span></span>
<span data-ttu-id="b40bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b40bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="b40bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b40bf-109">Permission type</span></span>      | <span data-ttu-id="b40bf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b40bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b40bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b40bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b40bf-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b40bf-112">Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="b40bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b40bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b40bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b40bf-114">Not supported.</span></span>    |
|<span data-ttu-id="b40bf-115">Application</span><span class="sxs-lookup"><span data-stu-id="b40bf-115">Application</span></span> | <span data-ttu-id="b40bf-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b40bf-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b40bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b40bf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/columns/{column-id}
DELETE /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```
## <a name="request-headers"></a><span data-ttu-id="b40bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b40bf-118">Request headers</span></span>
|<span data-ttu-id="b40bf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b40bf-119">Name</span></span>|<span data-ttu-id="b40bf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b40bf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b40bf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b40bf-121">Authorization</span></span>|<span data-ttu-id="b40bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b40bf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b40bf-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b40bf-124">Request body</span></span>
<span data-ttu-id="b40bf-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b40bf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b40bf-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b40bf-126">Response</span></span>

<span data-ttu-id="b40bf-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b40bf-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b40bf-128">Пример</span><span class="sxs-lookup"><span data-stu-id="b40bf-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="b40bf-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b40bf-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b40bf-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b40bf-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_columns_from_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```
# <a name="c"></a>[<span data-ttu-id="b40bf-131">C#</span><span class="sxs-lookup"><span data-stu-id="b40bf-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-columns-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b40bf-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b40bf-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-columns-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b40bf-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b40bf-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-columns-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b40bf-134">Java</span><span class="sxs-lookup"><span data-stu-id="b40bf-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-columns-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b40bf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b40bf-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[columndefinition]: ../resources/columndefinition.md
[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
