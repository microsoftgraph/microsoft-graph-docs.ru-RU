---
author: swapnil1993
title: 'contentType: публикация'
description: Публикация типа контента, присутствуют на сайте концентратора типов контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 2137c9fe371103d68785e67cfc815a15dba2ec54
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770445"
---
# <a name="contenttype-publish"></a><span data-ttu-id="0f8db-103">contentType: публикация</span><span class="sxs-lookup"><span data-stu-id="0f8db-103">contentType: publish</span></span>
<span data-ttu-id="0f8db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f8db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="0f8db-105">Публикует [контентТип,][] присутствующий на сайте концентратора типов контента.</span><span class="sxs-lookup"><span data-stu-id="0f8db-105">Publishes a [contentType][] present in content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f8db-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f8db-106">Permissions</span></span>

<span data-ttu-id="0f8db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f8db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="0f8db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f8db-109">Permission type</span></span>      | <span data-ttu-id="0f8db-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f8db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f8db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f8db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f8db-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0f8db-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="0f8db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f8db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f8db-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0f8db-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="0f8db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f8db-115">Application</span></span> | <span data-ttu-id="0f8db-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0f8db-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f8db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f8db-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/publish
```

><span data-ttu-id="0f8db-118">**Примечание:** SiteId представляет веб-узел типа контента.</span><span class="sxs-lookup"><span data-stu-id="0f8db-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f8db-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f8db-119">Request headers</span></span>
|<span data-ttu-id="0f8db-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0f8db-120">Name</span></span>|<span data-ttu-id="0f8db-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0f8db-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0f8db-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f8db-122">Authorization</span></span>|<span data-ttu-id="0f8db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f8db-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f8db-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f8db-125">Request body</span></span>
<span data-ttu-id="0f8db-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f8db-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f8db-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f8db-127">Response</span></span>
<span data-ttu-id="0f8db-128">В случае успешного ответа этот вызов возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="0f8db-128">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="0f8db-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0f8db-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f8db-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f8db-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0f8db-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f8db-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_publish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/publish
```
# <a name="c"></a>[<span data-ttu-id="0f8db-132">C#</span><span class="sxs-lookup"><span data-stu-id="0f8db-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f8db-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f8db-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f8db-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f8db-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f8db-135">Java</span><span class="sxs-lookup"><span data-stu-id="0f8db-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f8db-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f8db-136">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
