---
title: Получение ресурса ListItemVersion
description: В этой статье рассказывается, как получить метаданные для определенной версии ресурса ListItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c0c91c44b61b980da8a498b7f15ae6b71a42562e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460702"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="f4b60-103">Получение ресурса ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="f4b60-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="f4b60-104">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="f4b60-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4b60-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4b60-105">Permissions</span></span>

<span data-ttu-id="f4b60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="f4b60-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4b60-108">Permission type</span></span>             | <span data-ttu-id="f4b60-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4b60-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f4b60-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4b60-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4b60-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4b60-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="f4b60-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4b60-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4b60-113">Н/д</span><span class="sxs-lookup"><span data-stu-id="f4b60-113">n/a</span></span>                                         |
| <span data-ttu-id="f4b60-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4b60-114">Application</span></span>                            | <span data-ttu-id="f4b60-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4b60-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="f4b60-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4b60-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="f4b60-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4b60-117">Response</span></span>

<span data-ttu-id="f4b60-118">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4b60-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="f4b60-119">Пример</span><span class="sxs-lookup"><span data-stu-id="f4b60-119">Example</span></span>

<span data-ttu-id="f4b60-120">В этом примере показано, как получить версию объекта listItem и расширить коллекцию полей для запроса значений полей в объекте listItem.</span><span class="sxs-lookup"><span data-stu-id="f4b60-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="f4b60-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4b60-121">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f4b60-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4b60-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4b60-123">C#</span><span class="sxs-lookup"><span data-stu-id="f4b60-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4b60-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4b60-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4b60-125">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f4b60-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4b60-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4b60-126">Response</span></span>

<span data-ttu-id="f4b60-127">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="f4b60-127">This returns a collection of versions:</span></span>

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
