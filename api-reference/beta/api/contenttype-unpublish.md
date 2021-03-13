---
author: swapnil1993
title: 'contentType: неопубликованный'
description: Отопубликуй тип контента с сайта концентратора типа контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8b7e8c63c6d92390731b670f8d95821fe5334b0d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773384"
---
# <a name="contenttype-unpublish"></a><span data-ttu-id="ec35b-103">contentType: неопубликованный</span><span class="sxs-lookup"><span data-stu-id="ec35b-103">contentType: unpublish</span></span>
<span data-ttu-id="ec35b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec35b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="ec35b-105">Unpublish a [contentType][] from a content type hub site.</span><span class="sxs-lookup"><span data-stu-id="ec35b-105">Unpublish a [contentType][] from a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec35b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec35b-106">Permissions</span></span>

<span data-ttu-id="ec35b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec35b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="ec35b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec35b-109">Permission type</span></span>      | <span data-ttu-id="ec35b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec35b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec35b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec35b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ec35b-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ec35b-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="ec35b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec35b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec35b-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ec35b-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="ec35b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec35b-115">Application</span></span> | <span data-ttu-id="ec35b-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ec35b-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec35b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec35b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

><span data-ttu-id="ec35b-118">**Примечание:** SiteId представляет веб-узел типа контента.</span><span class="sxs-lookup"><span data-stu-id="ec35b-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec35b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec35b-119">Request headers</span></span>
|<span data-ttu-id="ec35b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ec35b-120">Name</span></span>|<span data-ttu-id="ec35b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ec35b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ec35b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec35b-122">Authorization</span></span>|<span data-ttu-id="ec35b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec35b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec35b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec35b-125">Request body</span></span>
<span data-ttu-id="ec35b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec35b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec35b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec35b-127">Response</span></span>

<span data-ttu-id="ec35b-128">В случае успешной работы этот метод возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="ec35b-128">If successful, this method returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="ec35b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ec35b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec35b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec35b-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ec35b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec35b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_unpublish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```
# <a name="c"></a>[<span data-ttu-id="ec35b-132">C#</span><span class="sxs-lookup"><span data-stu-id="ec35b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec35b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec35b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec35b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec35b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec35b-135">Java</span><span class="sxs-lookup"><span data-stu-id="ec35b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-unpublish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec35b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec35b-136">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
