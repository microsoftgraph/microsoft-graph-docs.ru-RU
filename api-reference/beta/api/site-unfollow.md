---
author: learafa
title: Отписаться от сайта
description: Отменять подписку на сайт пользователя
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: efb5862b38a5e8f0da651383aa935295dbc3dac1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271563"
---
# <a name="unfollow-site"></a><span data-ttu-id="72bba-103">Отписаться от сайта</span><span class="sxs-lookup"><span data-stu-id="72bba-103">Unfollow site</span></span> 

<span data-ttu-id="72bba-104">Отменяйте подписку на [сайт](../resources/site.md) пользователя или несколько сайтов.</span><span class="sxs-lookup"><span data-stu-id="72bba-104">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="72bba-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72bba-105">Permissions</span></span>

<span data-ttu-id="72bba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="72bba-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72bba-108">Permission type</span></span>             | <span data-ttu-id="72bba-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72bba-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="72bba-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72bba-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="72bba-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bba-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="72bba-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72bba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72bba-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72bba-113">Not supported.</span></span>                              |
| <span data-ttu-id="72bba-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72bba-114">Application</span></span>                            | <span data-ttu-id="72bba-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bba-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="72bba-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72bba-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="72bba-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72bba-117">Request body</span></span>

<span data-ttu-id="72bba-118">В теле запроса добавьте массив объектов JSON с параметром ID, указанным в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="72bba-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="72bba-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72bba-119">Name</span></span>                 | <span data-ttu-id="72bba-120">Значение</span><span class="sxs-lookup"><span data-stu-id="72bba-120">Value</span></span>  | <span data-ttu-id="72bba-121">Описание</span><span class="sxs-lookup"><span data-stu-id="72bba-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="72bba-122">id</span><span class="sxs-lookup"><span data-stu-id="72bba-122">id</span></span>                 | <span data-ttu-id="72bba-123">string</span><span class="sxs-lookup"><span data-stu-id="72bba-123">string</span></span> | <span data-ttu-id="72bba-124">[Уникальный идентификатор](../resources/site.md#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="72bba-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="72bba-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="72bba-125">Response</span></span>

* <span data-ttu-id="72bba-126">Если запрос выполнен успешно, этот метод возвращает код `204` состояния без содержимого.</span><span class="sxs-lookup"><span data-stu-id="72bba-126">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="72bba-127">Если при невозможности отследовать от указанных сайтов возникла ошибка, этот метод возвращает `207` код состояния, а текст отклика будет содержать массив записей, содержащих объекты [Error](/graph/errors) , и ситеидс, указывающие, какие сайты не могут быть отключены.</span><span class="sxs-lookup"><span data-stu-id="72bba-127">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="72bba-128">Пример</span><span class="sxs-lookup"><span data-stu-id="72bba-128">Example</span></span>

<span data-ttu-id="72bba-129">В приведенном ниже примере показано, как отписаться от нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="72bba-129">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="72bba-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="72bba-130">Request</span></span>

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
### <a name="response"></a><span data-ttu-id="72bba-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="72bba-131">Response</span></span>

<span data-ttu-id="72bba-132">В случае успешного выполнения возвращается следующий ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="72bba-132">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="72bba-133">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="72bba-133">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="72bba-134">C#</span><span class="sxs-lookup"><span data-stu-id="72bba-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/unfollow-site-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72bba-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="72bba-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/unfollow-site-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="72bba-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="72bba-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/unfollow-site-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="72bba-137">Если возникла ошибка, возвращается следующий ответ JSON</span><span class="sxs-lookup"><span data-stu-id="72bba-137">If an error occured, it returns the following JSON response</span></span> 

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
    "Error: /api-reference/beta/api/site-unfollow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/site-unfollow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/site-unfollow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
} -->
