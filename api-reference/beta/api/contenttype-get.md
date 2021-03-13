---
author: swapnil1993
title: Get contentType
description: Получите тип контента на сайте или в списке.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: a3dabf343ee4aef7c913cbcfa1bb6179b764fcf2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770612"
---
# <a name="get-contenttype"></a><span data-ttu-id="684c6-103">Get contentType</span><span class="sxs-lookup"><span data-stu-id="684c6-103">Get contentType</span></span>
<span data-ttu-id="684c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="684c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="684c6-105">Извлечение метаданных для типа [контента][contentType] на [сайте][] или в [списке.][]</span><span class="sxs-lookup"><span data-stu-id="684c6-105">Retrieve the metadata for a [content type][contentType] in a [site][] or a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="684c6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="684c6-106">Permissions</span></span>

<span data-ttu-id="684c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="684c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="684c6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="684c6-109">Permission type</span></span>      | <span data-ttu-id="684c6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="684c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="684c6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="684c6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="684c6-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="684c6-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="684c6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="684c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="684c6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="684c6-114">Not supported.</span></span>    |
|<span data-ttu-id="684c6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="684c6-115">Application</span></span> | <span data-ttu-id="684c6-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="684c6-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="684c6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="684c6-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes/{contentType-id}

GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="684c6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="684c6-118">Optional query parameters</span></span>
<span data-ttu-id="684c6-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="684c6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="684c6-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="684c6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="684c6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="684c6-121">Request headers</span></span>
|<span data-ttu-id="684c6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="684c6-122">Name</span></span>|<span data-ttu-id="684c6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="684c6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="684c6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="684c6-124">Authorization</span></span>|<span data-ttu-id="684c6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="684c6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="684c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="684c6-127">Request body</span></span>
<span data-ttu-id="684c6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="684c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="684c6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="684c6-129">Response</span></span>

<span data-ttu-id="684c6-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект contentType](../resources/contenttype.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="684c6-130">If successful, this method returns a `200 OK` response code and a [contentType](../resources/contenttype.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="684c6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="684c6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="684c6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="684c6-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="684c6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="684c6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contenttype"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
```
# <a name="c"></a>[<span data-ttu-id="684c6-134">C#</span><span class="sxs-lookup"><span data-stu-id="684c6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="684c6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="684c6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="684c6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="684c6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="684c6-137">Java</span><span class="sxs-lookup"><span data-stu-id="684c6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="684c6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="684c6-138">Response</span></span>
><span data-ttu-id="684c6-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="684c6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id":"0x0120D520",
  "description":"Create a document set when you want to manage multiple documents as a single work product.",
  "group":"Document Set Content Types",
  "hidden":false,
  "name":"Document Set",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```

[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
[list]: ../resources/list.md
