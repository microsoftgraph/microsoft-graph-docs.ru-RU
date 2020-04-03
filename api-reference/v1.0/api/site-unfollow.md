---
author: learafa
title: Прекращение отслеживания сайта
description: Отменять подписку на сайт пользователя
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 34ab2a05039cd509966175e36a9f5cedc873bc75
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125045"
---
# <a name="unfollow-site"></a><span data-ttu-id="e1dd4-103">Прекращение отслеживания сайта</span><span class="sxs-lookup"><span data-stu-id="e1dd4-103">Unfollow site</span></span> 

<span data-ttu-id="e1dd4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1dd4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1dd4-105">Отменяйте подписку на [сайт](../resources/site.md) пользователя или несколько сайтов.</span><span class="sxs-lookup"><span data-stu-id="e1dd4-105">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1dd4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1dd4-106">Permissions</span></span>

<span data-ttu-id="e1dd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1dd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="e1dd4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1dd4-109">Permission type</span></span>             | <span data-ttu-id="e1dd4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1dd4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e1dd4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1dd4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1dd4-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1dd4-112">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="e1dd4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1dd4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1dd4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1dd4-114">Not supported.</span></span>                              |
| <span data-ttu-id="e1dd4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1dd4-115">Application</span></span>                            | <span data-ttu-id="e1dd4-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1dd4-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e1dd4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1dd4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="e1dd4-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1dd4-118">Request body</span></span>

<span data-ttu-id="e1dd4-119">В теле запроса добавьте массив объектов JSON с параметром ID, указанным в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="e1dd4-119">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="e1dd4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e1dd4-120">Name</span></span>                 | <span data-ttu-id="e1dd4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e1dd4-121">Value</span></span>  | <span data-ttu-id="e1dd4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e1dd4-122">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="e1dd4-123">id</span><span class="sxs-lookup"><span data-stu-id="e1dd4-123">id</span></span>                 | <span data-ttu-id="e1dd4-124">строка</span><span class="sxs-lookup"><span data-stu-id="e1dd4-124">string</span></span> | <span data-ttu-id="e1dd4-125">[Уникальный идентификатор](../resources/site.md#id-property) элемента.</span><span class="sxs-lookup"><span data-stu-id="e1dd4-125">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="e1dd4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1dd4-126">Response</span></span>

* <span data-ttu-id="e1dd4-127">Если запрос выполнен успешно, этот метод возвращает код `204` состояния без содержимого.</span><span class="sxs-lookup"><span data-stu-id="e1dd4-127">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="e1dd4-128">Если при невозможности отследовать от указанных сайтов возникла ошибка, этот метод возвращает `207` код состояния, а текст отклика будет содержать массив записей, содержащих объекты [Error](/graph/errors) , и ситеидс, указывающие, какие сайты не могут быть отключены.</span><span class="sxs-lookup"><span data-stu-id="e1dd4-128">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="e1dd4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e1dd4-129">Example</span></span>

<span data-ttu-id="e1dd4-130">В приведенном ниже примере показано, как отписаться от нескольких сайтов.</span><span class="sxs-lookup"><span data-stu-id="e1dd4-130">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="e1dd4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1dd4-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e1dd4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1dd4-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e1dd4-133">C#</span><span class="sxs-lookup"><span data-stu-id="e1dd4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1dd4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1dd4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1dd4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1dd4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1dd4-136">Java</span><span class="sxs-lookup"><span data-stu-id="e1dd4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1dd4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1dd4-137">Response</span></span>

<span data-ttu-id="e1dd4-138">В случае успешного выполнения возвращается следующий ответ JSON.</span><span class="sxs-lookup"><span data-stu-id="e1dd4-138">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```

<span data-ttu-id="e1dd4-139">Если возникла ошибка, возвращается следующий ответ JSON</span><span class="sxs-lookup"><span data-stu-id="e1dd4-139">If an error occured, it returns the following JSON response</span></span> 

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
