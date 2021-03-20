---
author: swapnil1993
title: 'contentType: addCopy'
description: Добавьте копию типа контента сайта в список.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: f388799e409a5f2037182bb3bc331a6a6adbc45f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947032"
---
# <a name="contenttype-addcopy"></a><span data-ttu-id="56e51-103">contentType: addCopy</span><span class="sxs-lookup"><span data-stu-id="56e51-103">contentType: addCopy</span></span>
<span data-ttu-id="56e51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56e51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="56e51-105">Добавьте копию контента [типа][контентаType] с сайта [в][site] [список][list].</span><span class="sxs-lookup"><span data-stu-id="56e51-105">Add a copy of a [content type][contentType] from a [site][site] to a [list][list].</span></span>
 
  

## <a name="permissions"></a><span data-ttu-id="56e51-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56e51-106">Permissions</span></span>  

<span data-ttu-id="56e51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56e51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="56e51-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56e51-109">Permission type</span></span> | <span data-ttu-id="56e51-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56e51-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56e51-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56e51-111">Delegated (work or school account)</span></span> |<span data-ttu-id="56e51-112">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="56e51-112">Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="56e51-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56e51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56e51-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56e51-114">Not supported.</span></span> |
|<span data-ttu-id="56e51-115">Application</span><span class="sxs-lookup"><span data-stu-id="56e51-115">Application</span></span> | <span data-ttu-id="56e51-116">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="56e51-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="56e51-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56e51-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{site-id}/lists/{list-id}/contentTypes/addCopy
```

## <a name="request-headers"></a><span data-ttu-id="56e51-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56e51-118">Request headers</span></span>
|<span data-ttu-id="56e51-119">Имя</span><span class="sxs-lookup"><span data-stu-id="56e51-119">Name</span></span>|<span data-ttu-id="56e51-120">Описание</span><span class="sxs-lookup"><span data-stu-id="56e51-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="56e51-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56e51-121">Authorization</span></span>|<span data-ttu-id="56e51-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56e51-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="56e51-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56e51-124">Content-Type</span></span>|<span data-ttu-id="56e51-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56e51-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56e51-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56e51-127">Request body</span></span>
<span data-ttu-id="56e51-128">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="56e51-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="56e51-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="56e51-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="56e51-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="56e51-130">Parameter</span></span>|<span data-ttu-id="56e51-131">Тип</span><span class="sxs-lookup"><span data-stu-id="56e51-131">Type</span></span>|<span data-ttu-id="56e51-132">Описание</span><span class="sxs-lookup"><span data-stu-id="56e51-132">Description</span></span>|
|-|-|-|
|<span data-ttu-id="56e51-133">contentType</span><span class="sxs-lookup"><span data-stu-id="56e51-133">contentType</span></span>| <span data-ttu-id="56e51-134">string</span><span class="sxs-lookup"><span data-stu-id="56e51-134">string</span></span> | <span data-ttu-id="56e51-135">Канонический URL-адрес типа контента сайта, который будет скопирован в список.</span><span class="sxs-lookup"><span data-stu-id="56e51-135">Canonical URL to the site content type that will be copied to the list.</span></span> <span data-ttu-id="56e51-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56e51-136">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="56e51-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="56e51-137">Response</span></span>

<span data-ttu-id="56e51-138">В случае успешного ответа этот вызов возвращает код отклика и `201 Created` [объект contentType][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="56e51-138">If successful, this call returns a `201 Created` response code and a [contentType][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56e51-139">Пример</span><span class="sxs-lookup"><span data-stu-id="56e51-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="56e51-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="56e51-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="56e51-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="56e51-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopy"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/lists/{list-id}/contentTypes/addCopy
Content-Type: application/json

{
  "contentType": "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
}
```
# <a name="c"></a>[<span data-ttu-id="56e51-142">C#</span><span class="sxs-lookup"><span data-stu-id="56e51-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-addcopy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56e51-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56e51-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-addcopy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56e51-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56e51-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-addcopy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56e51-145">Java</span><span class="sxs-lookup"><span data-stu-id="56e51-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-addcopy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="56e51-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="56e51-146">Response</span></span>


<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

```http
HTTP/1.1 201 Created

{
    "id": "0x0101",
    "description": "Create a new custom CSR JavaScript Display Template.",
    "group": "Display Template Content Types",
    "hidden": false,
    "name": "JavaScript Display Template",
    "parentId": "0x01",
    "readOnly": false,
    "sealed": false,
    "base": {
        "id": "0x01",
        "description": "Create a new custom CSR JavaScript Display Template.",
        "group": "Display Template Content Types",
        "hidden": false,
        "name": "JavaScript Display Template",
        "readOnly": false,
        "sealed": false
    }
}
```

[site]: ../resources/site.md
[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
