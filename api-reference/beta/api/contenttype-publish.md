---
author: swapnil1993
title: 'contentType: публикация'
description: Публикация типа контента, присутствуют на сайте концентратора типов контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: d69cbdabbb82612945dc6df85617e50bc2ca5b2c
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467087"
---
# <a name="contenttype-publish"></a><span data-ttu-id="bf080-103">contentType: публикация</span><span class="sxs-lookup"><span data-stu-id="bf080-103">contentType: publish</span></span>
<span data-ttu-id="bf080-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf080-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="bf080-105">Публикует [контентТип,][] присутствующий на сайте концентратора типов контента.</span><span class="sxs-lookup"><span data-stu-id="bf080-105">Publishes a [contentType][] present in a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf080-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf080-106">Permissions</span></span>

<span data-ttu-id="bf080-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="bf080-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf080-109">Permission type</span></span>      | <span data-ttu-id="bf080-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf080-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf080-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf080-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf080-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bf080-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="bf080-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf080-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf080-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bf080-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="bf080-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="bf080-115">Application</span></span> | <span data-ttu-id="bf080-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bf080-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf080-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf080-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/publish
```

><span data-ttu-id="bf080-118">**Примечание:** `siteId` представляет веб-узел типа контента.</span><span class="sxs-lookup"><span data-stu-id="bf080-118">**Note:** `siteId` represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf080-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf080-119">Request headers</span></span>
|<span data-ttu-id="bf080-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bf080-120">Name</span></span>|<span data-ttu-id="bf080-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bf080-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bf080-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf080-122">Authorization</span></span>|<span data-ttu-id="bf080-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf080-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf080-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf080-125">Request body</span></span>
<span data-ttu-id="bf080-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf080-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf080-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf080-127">Response</span></span>
<span data-ttu-id="bf080-128">В случае успешного ответа этот вызов возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="bf080-128">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="bf080-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bf080-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf080-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf080-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bf080-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf080-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_publish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/publish
```
# <a name="c"></a>[<span data-ttu-id="bf080-132">C#</span><span class="sxs-lookup"><span data-stu-id="bf080-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf080-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf080-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf080-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf080-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf080-135">Java</span><span class="sxs-lookup"><span data-stu-id="bf080-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bf080-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf080-136">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
