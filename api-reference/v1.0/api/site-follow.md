---
author: learafa
title: Отслеживание сайта
description: Подпишитесь на сайт или сайты пользователя.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 07acd4f0baf9cf1450605a4b5fc7a4775ba06df9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038216"
---
# <a name="follow-site"></a><span data-ttu-id="ca2b2-103">Отслеживание сайта</span><span class="sxs-lookup"><span data-stu-id="ca2b2-103">Follow site</span></span> 

<span data-ttu-id="ca2b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca2b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca2b2-105">Подпишитесь на [сайт](../resources/site.md) пользователя или несколько сайтов.</span><span class="sxs-lookup"><span data-stu-id="ca2b2-105">Follow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca2b2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca2b2-106">Permissions</span></span>

<span data-ttu-id="ca2b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca2b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="ca2b2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca2b2-109">Permission type</span></span>             | <span data-ttu-id="ca2b2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca2b2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ca2b2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca2b2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca2b2-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2b2-112">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="ca2b2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca2b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca2b2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca2b2-114">Not supported.</span></span>                              |
| <span data-ttu-id="ca2b2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca2b2-115">Application</span></span>                            | <span data-ttu-id="ca2b2-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2b2-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ca2b2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca2b2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/add
```

## <a name="request-body"></a><span data-ttu-id="ca2b2-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca2b2-118">Request body</span></span>

<span data-ttu-id="ca2b2-119">В теле запроса добавьте массив объектов JSON с параметром ID, указанным в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="ca2b2-119">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="ca2b2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ca2b2-120">Name</span></span>                 | <span data-ttu-id="ca2b2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ca2b2-121">Value</span></span>  | <span data-ttu-id="ca2b2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2b2-122">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="ca2b2-123">id</span><span class="sxs-lookup"><span data-stu-id="ca2b2-123">id</span></span>                 | <span data-ttu-id="ca2b2-124">string</span><span class="sxs-lookup"><span data-stu-id="ca2b2-124">string</span></span> | <span data-ttu-id="ca2b2-125">[Уникальный идентификатор](../resources/site.md#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="ca2b2-125">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |


## <a name="response"></a><span data-ttu-id="ca2b2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca2b2-126">Response</span></span> 

* <span data-ttu-id="ca2b2-127">Если запрос выполнен успешно, этот метод возвращает массив сайтов, которые были выполнены.</span><span class="sxs-lookup"><span data-stu-id="ca2b2-127">If the request is successful, this method returns an array of sites that were followed.</span></span>  
* <span data-ttu-id="ca2b2-128">Если при выполнении какого-либо из указанных сайтов возникла ошибка, этот метод возвращает `207` код состояния, а текст отклика будет содержать массив записей, содержащих объекты [Error](/graph/errors) , и ситеидс, указывающие, какие сайты не могут быть выполнены.</span><span class="sxs-lookup"><span data-stu-id="ca2b2-128">If an error occurred while following any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites were unable to be followed.</span></span>

## <a name="example"></a><span data-ttu-id="ca2b2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ca2b2-129">Example</span></span>

<span data-ttu-id="ca2b2-130">В приведенном ниже примере показано, как подписаться на несколько сайтов.</span><span class="sxs-lookup"><span data-stu-id="ca2b2-130">The following example shows how to follow multiple sites.</span></span> 

### <a name="request"></a><span data-ttu-id="ca2b2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca2b2-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ca2b2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca2b2-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-site", "scopes": "sites.readwrite.all" } -->

```http
POST /users/{user-id}/followedSites/add
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
# <a name="c"></a>[<span data-ttu-id="ca2b2-133">C#</span><span class="sxs-lookup"><span data-stu-id="ca2b2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca2b2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca2b2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca2b2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca2b2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca2b2-136">Java</span><span class="sxs-lookup"><span data-stu-id="ca2b2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/follow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ca2b2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca2b2-137">Response</span></span>

<span data-ttu-id="ca2b2-138">В случае успешного выполнения возвращается следующий ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="ca2b2-138">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed1",
            "name": "SiteFollowed1",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed1",
                "webId": "712a596e-90a1-49e3-9b48-bfa80bee8740"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
            "name": "SiteFollowed2",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
                "webId": "0271110f-634f-4300-a841-3a8a2e851851"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
    ]
}
```

<span data-ttu-id="ca2b2-139">Если возникла ошибка, возвращается следующий ответ JSON</span><span class="sxs-lookup"><span data-stu-id="ca2b2-139">If an error occured, it returns the following JSON response</span></span> 

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
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
            "name": "SiteFollowed2",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
                "webId": "0271110f-634f-4300-a841-3a8a2e851851"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
    ]
}
```  

<!-- {
  "type": "#page.annotation",
  "description": "Follow sharepoint site for a user.",
  "keywords": "follow site",
  "section": "documentation",
  "tocPath": "Sites/Follow site",
  "suppressions": [
  ]
} -->

