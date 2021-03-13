---
author: swapnil1993
title: 'contentType: addCopy'
description: Добавьте копию типа контента сайта в список.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 97c93929fbc0c370bd4dac53b068439f5bbd5b82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771150"
---
# <a name="contenttype-addcopy"></a><span data-ttu-id="9891b-103">contentType: addCopy</span><span class="sxs-lookup"><span data-stu-id="9891b-103">contentType: addCopy</span></span>
<span data-ttu-id="9891b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9891b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="9891b-105">Добавьте копию типа [контента][site] [сайта][contentType] в [список][list].</span><span class="sxs-lookup"><span data-stu-id="9891b-105">Add a copy of a [site][site] [content type][contentType] to a [list][list].</span></span>
 
  

## <a name="permissions"></a><span data-ttu-id="9891b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9891b-106">Permissions</span></span>  

<span data-ttu-id="9891b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9891b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="9891b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9891b-109">Permission type</span></span> | <span data-ttu-id="9891b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9891b-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9891b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9891b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9891b-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="9891b-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="9891b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9891b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9891b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9891b-114">Not supported.</span></span> |
|<span data-ttu-id="9891b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9891b-115">Application</span></span> | <span data-ttu-id="9891b-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="9891b-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="9891b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9891b-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http

POST /sites/{site-id}/lists/{list-id}/contentTypes/addCopy
```

## <a name="request-headers"></a><span data-ttu-id="9891b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9891b-118">Request headers</span></span>
|<span data-ttu-id="9891b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9891b-119">Name</span></span>|<span data-ttu-id="9891b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9891b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9891b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9891b-121">Authorization</span></span>|<span data-ttu-id="9891b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9891b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9891b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9891b-124">Content-Type</span></span>|<span data-ttu-id="9891b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9891b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9891b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9891b-127">Request body</span></span>
<span data-ttu-id="9891b-128">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="9891b-128">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="9891b-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9891b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9891b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="9891b-130">Parameter</span></span>|<span data-ttu-id="9891b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9891b-131">Type</span></span>|<span data-ttu-id="9891b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9891b-132">Description</span></span>|
|-|-|-|
|<span data-ttu-id="9891b-133">contentType</span><span class="sxs-lookup"><span data-stu-id="9891b-133">contentType</span></span>| <span data-ttu-id="9891b-134">string</span><span class="sxs-lookup"><span data-stu-id="9891b-134">string</span></span> | <span data-ttu-id="9891b-135">Канонический URL-адрес типа контента сайта, который будет скопирован в список.</span><span class="sxs-lookup"><span data-stu-id="9891b-135">Canonical URL to the site content type that will be copied to the list.</span></span> <span data-ttu-id="9891b-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9891b-136">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="9891b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9891b-137">Response</span></span>

<span data-ttu-id="9891b-138">В случае успешного ответа этот вызов возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="9891b-138">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="9891b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9891b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="9891b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9891b-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9891b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="9891b-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9891b-142">C#</span><span class="sxs-lookup"><span data-stu-id="9891b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-addcopy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9891b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9891b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-addcopy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9891b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9891b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-addcopy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9891b-145">Java</span><span class="sxs-lookup"><span data-stu-id="9891b-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-addcopy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="9891b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="9891b-146">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content

```

[site]: ../resources/site.md
[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
