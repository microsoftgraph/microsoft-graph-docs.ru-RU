---
author: learafa
title: Отписаться от сайта
description: Отменять подписку на сайт пользователя
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: de1237c26c259eca72b7a800ca1842d9203c7eec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869603"
---
# <a name="unfollow-site"></a><span data-ttu-id="73ca6-103">Отписаться от сайта</span><span class="sxs-lookup"><span data-stu-id="73ca6-103">Unfollow site</span></span> 

<span data-ttu-id="73ca6-104">Отменяйте подписку на [сайт](../resources/site.md) пользователя или несколько сайтов.</span><span class="sxs-lookup"><span data-stu-id="73ca6-104">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="73ca6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73ca6-105">Permissions</span></span>

<span data-ttu-id="73ca6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73ca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="73ca6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73ca6-108">Permission type</span></span>             | <span data-ttu-id="73ca6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73ca6-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="73ca6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73ca6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="73ca6-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ca6-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="73ca6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73ca6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73ca6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73ca6-113">Not supported.</span></span>                              |
| <span data-ttu-id="73ca6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73ca6-114">Application</span></span>                            | <span data-ttu-id="73ca6-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ca6-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="73ca6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73ca6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="73ca6-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73ca6-117">Request body</span></span>

<span data-ttu-id="73ca6-118">В теле запроса добавьте массив объектов JSON с параметром ID, указанным в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="73ca6-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="73ca6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="73ca6-119">Name</span></span>                 | <span data-ttu-id="73ca6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="73ca6-120">Value</span></span>  | <span data-ttu-id="73ca6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="73ca6-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="73ca6-122">id</span><span class="sxs-lookup"><span data-stu-id="73ca6-122">id</span></span>                 | <span data-ttu-id="73ca6-123">string</span><span class="sxs-lookup"><span data-stu-id="73ca6-123">string</span></span> | <span data-ttu-id="73ca6-124">[Уникальный идентификатор](../resources/site.md#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="73ca6-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="73ca6-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="73ca6-125">Response</span></span>

* <span data-ttu-id="73ca6-126">Если запрос выполнен успешно, этот метод возвращает код `204` состояния без содержимого.</span><span class="sxs-lookup"><span data-stu-id="73ca6-126">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="73ca6-127">Если при невозможности отследовать от указанных сайтов возникла ошибка, этот метод возвращает `207` код состояния, а текст отклика будет содержать массив записей, содержащих объекты [Error](/graph/errors) , и ситеидс, указывающие, какие сайты не могут быть отключены.</span><span class="sxs-lookup"><span data-stu-id="73ca6-127">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="73ca6-128">Пример</span><span class="sxs-lookup"><span data-stu-id="73ca6-128">Example</span></span>

<span data-ttu-id="73ca6-129">В приведенном ниже примере показано, как отписаться от нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="73ca6-129">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="73ca6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="73ca6-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="73ca6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="73ca6-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="73ca6-132">C#</span><span class="sxs-lookup"><span data-stu-id="73ca6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73ca6-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="73ca6-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73ca6-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="73ca6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73ca6-135">Java</span><span class="sxs-lookup"><span data-stu-id="73ca6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="73ca6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="73ca6-136">Response</span></span>

<span data-ttu-id="73ca6-137">В случае успешного выполнения возвращается следующий ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="73ca6-137">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```

<span data-ttu-id="73ca6-138">Если возникла ошибка, возвращается следующий ответ JSON</span><span class="sxs-lookup"><span data-stu-id="73ca6-138">If an error occured, it returns the following JSON response</span></span> 

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
