---
author: swapnil1993
title: 'contentType: isPublished'
description: Проверьте состояние публикации типа контента на веб-узбе типа контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: e61d488dddc9797c3f0623a3e534f54b1bab4708
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439436"
---
# <a name="contenttype-ispublished"></a><span data-ttu-id="20867-103">contentType: isPublished</span><span class="sxs-lookup"><span data-stu-id="20867-103">contentType: isPublished</span></span>
<span data-ttu-id="20867-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20867-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="20867-105">Проверьте состояние публикации [контентаType][] на веб-сайте концентратора типа контента.</span><span class="sxs-lookup"><span data-stu-id="20867-105">Check the publishing status of a [contentType][] in a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="20867-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20867-106">Permissions</span></span>

<span data-ttu-id="20867-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20867-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20867-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20867-109">Permission type</span></span>      | <span data-ttu-id="20867-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20867-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20867-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20867-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20867-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="20867-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="20867-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20867-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20867-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="20867-114">Not Supported</span></span>   |
|<span data-ttu-id="20867-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="20867-115">Application</span></span> | <span data-ttu-id="20867-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="20867-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20867-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20867-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
><span data-ttu-id="20867-118">**Примечание:** _siteId_ представляет веб-узел типа контента.</span><span class="sxs-lookup"><span data-stu-id="20867-118">**Note:** _siteId_ represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20867-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20867-119">Request headers</span></span>
|<span data-ttu-id="20867-120">Имя</span><span class="sxs-lookup"><span data-stu-id="20867-120">Name</span></span>|<span data-ttu-id="20867-121">Описание</span><span class="sxs-lookup"><span data-stu-id="20867-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20867-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20867-122">Authorization</span></span>|<span data-ttu-id="20867-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20867-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="20867-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="20867-125">Response</span></span>
<span data-ttu-id="20867-126">В случае успешной работы этот вызов возвращает ответ и значение boolean, которое указывает состояние публикации `200 OK` типа контента.</span><span class="sxs-lookup"><span data-stu-id="20867-126">If successful, this call returns a `200 OK` response and a boolean value that specifies the publishing state of the content type.</span></span>

## <a name="request-body"></a><span data-ttu-id="20867-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20867-127">Request body</span></span>
<span data-ttu-id="20867-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20867-128">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="20867-129">Пример</span><span class="sxs-lookup"><span data-stu-id="20867-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="20867-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="20867-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="20867-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="20867-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_ispublished"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
# <a name="c"></a>[<span data-ttu-id="20867-132">C#</span><span class="sxs-lookup"><span data-stu-id="20867-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-ispublished-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20867-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20867-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-ispublished-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20867-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20867-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-ispublished-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20867-135">Java</span><span class="sxs-lookup"><span data-stu-id="20867-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-ispublished-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="20867-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="20867-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": true 
}
```

[contentType]: ../resources/contentType.md
