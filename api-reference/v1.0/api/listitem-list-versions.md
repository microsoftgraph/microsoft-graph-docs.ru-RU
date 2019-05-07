---
title: Перечисление версий элемента ListItem
description: Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9e0230ac732f39831894315ef86a7c1bcdfa10e0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613362"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="610df-103">Перечисление версий элемента ListItem</span><span class="sxs-lookup"><span data-stu-id="610df-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="610df-104">Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.</span><span class="sxs-lookup"><span data-stu-id="610df-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="610df-105">Предыдущие версии можно хранить в течение конечного периода времени, настроенного администратором. Такой период можно задавать отдельно для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="610df-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="610df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="610df-106">Permissions</span></span>

<span data-ttu-id="610df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="610df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="610df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="610df-109">Permission type</span></span>             | <span data-ttu-id="610df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="610df-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="610df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="610df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="610df-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="610df-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="610df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="610df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="610df-114">Н/д</span><span class="sxs-lookup"><span data-stu-id="610df-114">n/a</span></span>                                         |
| <span data-ttu-id="610df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="610df-115">Application</span></span>                            | <span data-ttu-id="610df-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="610df-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="610df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="610df-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="610df-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="610df-118">Response</span></span>

<span data-ttu-id="610df-119">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="610df-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="610df-120">Пример</span><span class="sxs-lookup"><span data-stu-id="610df-120">Example</span></span>

<span data-ttu-id="610df-121">В этом примере показано, как получить версии элемента listItem в списке SharePoint:</span><span class="sxs-lookup"><span data-stu-id="610df-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="610df-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="610df-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="610df-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="610df-123">Response</span></span>

<span data-ttu-id="610df-124">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="610df-124">This returns a collection of versions:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="610df-125">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="610df-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="610df-126">Языках</span><span class="sxs-lookup"><span data-stu-id="610df-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-previous-versions-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="610df-127">Язык</span><span class="sxs-lookup"><span data-stu-id="610df-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-previous-versions-listitem-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
