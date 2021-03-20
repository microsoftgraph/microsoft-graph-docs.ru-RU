---
author: swapnil1993
title: 'contentType: associateWithHubSites'
description: Связать тип контента со списком узлов.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: dbddfcd4f2f3fc94c9be4ebf30aeb0c8522ea855
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947018"
---
# <a name="contenttype-associatewithhubsites"></a><span data-ttu-id="ec748-103">contentType: associateWithHubSites</span><span class="sxs-lookup"><span data-stu-id="ec748-103">contentType: associateWithHubSites</span></span>

<span data-ttu-id="ec748-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec748-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="ec748-105">Связывать [тип контента][contentType] со списком сайтов-концентраторов.</span><span class="sxs-lookup"><span data-stu-id="ec748-105">Associate a [content type][contentType] with a list of hub sites.</span></span>

><span data-ttu-id="ec748-106">**Примечание:** Эта функция ограничена для клиентов с лицензией SharePoint Syntex.</span><span class="sxs-lookup"><span data-stu-id="ec748-106">**Note:** This feature is limited to tenants that have a SharePoint Syntex license.</span></span>
  

## <a name="permissions"></a><span data-ttu-id="ec748-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec748-107">Permissions</span></span>  

<span data-ttu-id="ec748-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="ec748-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec748-110">Permission type</span></span> | <span data-ttu-id="ec748-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec748-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------
|<span data-ttu-id="ec748-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec748-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec748-113">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ec748-113">Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="ec748-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec748-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec748-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec748-115">Not supported.</span></span> |
|<span data-ttu-id="ec748-116">Application</span><span class="sxs-lookup"><span data-stu-id="ec748-116">Application</span></span> | <span data-ttu-id="ec748-117">Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ec748-117">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="ec748-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec748-118">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/id/contentTypes/id/associateWithHubSites
```

## <a name="request-headers"></a><span data-ttu-id="ec748-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec748-119">Request headers</span></span>
|<span data-ttu-id="ec748-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ec748-120">Name</span></span>|<span data-ttu-id="ec748-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ec748-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ec748-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec748-122">Authorization</span></span>|<span data-ttu-id="ec748-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec748-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ec748-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec748-125">Content-Type</span></span>|<span data-ttu-id="ec748-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec748-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec748-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec748-128">Request body</span></span>
<span data-ttu-id="ec748-129">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="ec748-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="ec748-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ec748-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ec748-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="ec748-131">Parameter</span></span>|<span data-ttu-id="ec748-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ec748-132">Type</span></span>|<span data-ttu-id="ec748-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ec748-133">Description</span></span>|
|-|-|-|
|<span data-ttu-id="ec748-134">hubSiteUrls</span><span class="sxs-lookup"><span data-stu-id="ec748-134">hubSiteUrls</span></span>| <span data-ttu-id="ec748-135">Коллекция (строка)</span><span class="sxs-lookup"><span data-stu-id="ec748-135">Collection(string)</span></span> |<span data-ttu-id="ec748-136">Список пушечных URL-адресов для узлов, на которых необходимо применять тип контента.</span><span class="sxs-lookup"><span data-stu-id="ec748-136">List of cannonical URLs to the hub sites where the content type needs to be enforced.</span></span> <span data-ttu-id="ec748-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec748-137">Required.</span></span>|
|<span data-ttu-id="ec748-138">propagateToExistingLists</span><span class="sxs-lookup"><span data-stu-id="ec748-138">propagateToExistingLists</span></span>| <span data-ttu-id="ec748-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec748-139">Boolean</span></span> |<span data-ttu-id="ec748-140">Если типы контента будут применяться в существующих списках на сайтах концентратора; в противном случае он будет применяться только к вновь `true` созданным спискам.</span><span class="sxs-lookup"><span data-stu-id="ec748-140">If `true`, content types will be enforced on existing lists in the hub sites; otherwise, it will be applied only to newly created lists.</span></span> 

## <a name="response"></a><span data-ttu-id="ec748-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec748-141">Response</span></span>

<span data-ttu-id="ec748-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ec748-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ec748-143">Пример</span><span class="sxs-lookup"><span data-stu-id="ec748-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec748-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec748-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ec748-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec748-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_associatewithhubsites"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/contentTypes/id/associateWithHubSites
Content-Type: application/json

{
   "hubSiteUrls":[
      "https://graph.microsoft.com/beta/sites/id"
   ],
   "propagateToExistingLists":false
}
```
# <a name="c"></a>[<span data-ttu-id="ec748-146">C#</span><span class="sxs-lookup"><span data-stu-id="ec748-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-associatewithhubsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec748-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec748-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-associatewithhubsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec748-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec748-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-associatewithhubsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec748-149">Java</span><span class="sxs-lookup"><span data-stu-id="ec748-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-associatewithhubsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="ec748-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec748-150">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
