---
title: Получение ресурса ListItemVersion
description: В этой статье рассказывается, как получить метаданные для определенной версии ресурса ListItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 4a7e10787b23ab422a64a30db7d0d921edfdfbcf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511679"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="f8e19-103">Получение ресурса ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="f8e19-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="f8e19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8e19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8e19-105">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="f8e19-105">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8e19-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8e19-106">Permissions</span></span>

<span data-ttu-id="f8e19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8e19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="f8e19-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8e19-109">Permission type</span></span>             | <span data-ttu-id="f8e19-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8e19-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f8e19-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8e19-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8e19-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8e19-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="f8e19-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8e19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8e19-114">Н/д</span><span class="sxs-lookup"><span data-stu-id="f8e19-114">n/a</span></span>                                         |
| <span data-ttu-id="f8e19-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8e19-115">Application</span></span>                            | <span data-ttu-id="f8e19-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8e19-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="f8e19-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8e19-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="f8e19-118">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8e19-118">Response</span></span>

<span data-ttu-id="f8e19-119">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f8e19-119">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="f8e19-120">Пример</span><span class="sxs-lookup"><span data-stu-id="f8e19-120">Example</span></span>

<span data-ttu-id="f8e19-121">В этом примере показано, как получить версию объекта listItem и расширить коллекцию полей для запроса значений полей в объекте listItem.</span><span class="sxs-lookup"><span data-stu-id="f8e19-121">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="f8e19-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8e19-122">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="f8e19-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8e19-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="f8e19-124">C#</span><span class="sxs-lookup"><span data-stu-id="f8e19-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8e19-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8e19-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8e19-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8e19-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8e19-127">Java</span><span class="sxs-lookup"><span data-stu-id="f8e19-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8e19-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8e19-128">Response</span></span>

<span data-ttu-id="f8e19-129">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="f8e19-129">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
