---
author: learafa
title: Прекращение отслеживания сайта
description: Отменять подписку на сайт пользователя
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c15c8d05e688bd9c02455340f8f94d0f33939b26
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044496"
---
# <a name="unfollow-site"></a><span data-ttu-id="f79a0-103">Прекращение отслеживания сайта</span><span class="sxs-lookup"><span data-stu-id="f79a0-103">Unfollow site</span></span> 

<span data-ttu-id="f79a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f79a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f79a0-105">Отменяйте подписку на [сайт](../resources/site.md) пользователя или несколько сайтов.</span><span class="sxs-lookup"><span data-stu-id="f79a0-105">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="f79a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f79a0-106">Permissions</span></span>

<span data-ttu-id="f79a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f79a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="f79a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f79a0-109">Permission type</span></span>             | <span data-ttu-id="f79a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f79a0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f79a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f79a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f79a0-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f79a0-112">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="f79a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f79a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f79a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f79a0-114">Not supported.</span></span>                              |
| <span data-ttu-id="f79a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f79a0-115">Application</span></span>                            | <span data-ttu-id="f79a0-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f79a0-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f79a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f79a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="f79a0-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f79a0-118">Request body</span></span>

<span data-ttu-id="f79a0-119">В теле запроса добавьте массив объектов JSON с параметром ID, указанным в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="f79a0-119">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="f79a0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f79a0-120">Name</span></span>                 | <span data-ttu-id="f79a0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f79a0-121">Value</span></span>  | <span data-ttu-id="f79a0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f79a0-122">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="f79a0-123">id</span><span class="sxs-lookup"><span data-stu-id="f79a0-123">id</span></span>                 | <span data-ttu-id="f79a0-124">string</span><span class="sxs-lookup"><span data-stu-id="f79a0-124">string</span></span> | <span data-ttu-id="f79a0-125">[Уникальный идентификатор](../resources/site.md#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="f79a0-125">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="f79a0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f79a0-126">Response</span></span>

* <span data-ttu-id="f79a0-127">Если запрос выполнен успешно, этот метод возвращает `204` код состояния без содержимого.</span><span class="sxs-lookup"><span data-stu-id="f79a0-127">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="f79a0-128">Если при невозможности отследовать от указанных сайтов возникла ошибка, этот метод возвращает `207` код состояния, а текст отклика будет содержать массив записей, содержащих объекты [Error](/graph/errors) , и ситеидс, указывающие, какие сайты не могут быть отключены.</span><span class="sxs-lookup"><span data-stu-id="f79a0-128">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="f79a0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f79a0-129">Example</span></span>

<span data-ttu-id="f79a0-130">В приведенном ниже примере показано, как отписаться от нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="f79a0-130">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="f79a0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f79a0-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f79a0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f79a0-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-site", "scopes": "sites.readwrite.all" } -->

```http
POST /users/{user-id}/followedSites/remove
Content-Type: application/json

{
    "value":
    [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740"
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="f79a0-133">C#</span><span class="sxs-lookup"><span data-stu-id="f79a0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f79a0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f79a0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f79a0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f79a0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f79a0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f79a0-136">Response</span></span>

<span data-ttu-id="f79a0-137">В случае успешного выполнения возвращается следующий ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="f79a0-137">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```

<span data-ttu-id="f79a0-138">Если возникла ошибка, возвращается следующий ответ JSON</span><span class="sxs-lookup"><span data-stu-id="f79a0-138">If an error occured, it returns the following JSON response</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
    "value": [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,512a596e-90a1-49e3-9b48-bfa80bee8740",
            "error": {
                "@odata.type": "#oneDrive.error",
                "code": "invalidRequest",
                "message": "The site Id information that is provided in the request is incorrect",
                "innerError": {
                    "code": "invalidRequest",
                    "errorType": "expected",
                    "message": "The site Id information that is provided in the request is incorrect",
                    "stackTrace": "",
                    "throwSite": ""
                }
            }
        }
    ]
}
```  

<!-- {
  "type": "#page.annotation",
  "description": "Unfollow sharepoint site/sites for a user.",
  "keywords": "unfollow site",
  "section": "documentation",
  "tocPath": "Sites/Unfollow site",
  "suppressions": [
  ]
} -->


