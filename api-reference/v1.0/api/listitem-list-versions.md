---
title: Перечисление версий элемента ListItem
description: Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: b4a29ce4850ba45f89e2de7cd3fc07a3f6360dd7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730241"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="51ea4-103">Перечисление версий элемента ListItem</span><span class="sxs-lookup"><span data-stu-id="51ea4-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="51ea4-104">Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.</span><span class="sxs-lookup"><span data-stu-id="51ea4-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="51ea4-105">Предыдущие версии можно хранить в течение конечного периода времени, настроенного администратором. Такой период можно задавать отдельно для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="51ea4-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="51ea4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51ea4-106">Permissions</span></span>

<span data-ttu-id="51ea4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51ea4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="51ea4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51ea4-109">Permission type</span></span>             | <span data-ttu-id="51ea4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51ea4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="51ea4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51ea4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="51ea4-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ea4-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="51ea4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51ea4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51ea4-114">Н/д</span><span class="sxs-lookup"><span data-stu-id="51ea4-114">n/a</span></span>                                         |
| <span data-ttu-id="51ea4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51ea4-115">Application</span></span>                            | <span data-ttu-id="51ea4-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ea4-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="51ea4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51ea4-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="51ea4-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="51ea4-118">Response</span></span>

<span data-ttu-id="51ea4-119">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51ea4-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="51ea4-120">Пример</span><span class="sxs-lookup"><span data-stu-id="51ea4-120">Example</span></span>

<span data-ttu-id="51ea4-121">В этом примере показано, как получить версии элемента listItem в списке SharePoint:</span><span class="sxs-lookup"><span data-stu-id="51ea4-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="51ea4-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51ea4-122">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="51ea4-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="51ea4-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="51ea4-124">C#</span><span class="sxs-lookup"><span data-stu-id="51ea4-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51ea4-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51ea4-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51ea4-126">Цель — C</span><span class="sxs-lookup"><span data-stu-id="51ea4-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="51ea4-127">Java</span><span class="sxs-lookup"><span data-stu-id="51ea4-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="51ea4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="51ea4-128">Response</span></span>

<span data-ttu-id="51ea4-129">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="51ea4-129">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
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
