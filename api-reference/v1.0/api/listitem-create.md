---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание записи в списке SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e2183eff38bdf4237ab4464cfb6bd55e1f88fa16
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272032"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="814ed-102">Создание элемента в списке</span><span class="sxs-lookup"><span data-stu-id="814ed-102">Create a new item in a list</span></span>

<span data-ttu-id="814ed-103">Создание элемента [listItem][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="814ed-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="814ed-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="814ed-104">Permissions</span></span>

<span data-ttu-id="814ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="814ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="814ed-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="814ed-107">Permission type</span></span>      | <span data-ttu-id="814ed-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="814ed-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="814ed-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="814ed-109">Delegated (work or school account)</span></span> | <span data-ttu-id="814ed-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="814ed-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="814ed-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="814ed-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="814ed-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="814ed-112">Not supported.</span></span>    |
|<span data-ttu-id="814ed-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="814ed-113">Application</span></span> | <span data-ttu-id="814ed-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="814ed-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="814ed-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="814ed-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="814ed-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="814ed-116">Request body</span></span>

<span data-ttu-id="814ed-117">В теле запроса укажите представление ресурса [listItem][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="814ed-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="814ed-118">Пример</span><span class="sxs-lookup"><span data-stu-id="814ed-118">Example</span></span>

<span data-ttu-id="814ed-119">В примере ниже показано, как создать элемент списка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="814ed-119">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="814ed-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="814ed-120">Response</span></span>

<span data-ttu-id="814ed-121">При успешном выполнении этот метод возвращает объект [listItem][] для созданного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="814ed-121">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="814ed-122">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="814ed-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="814ed-123">C#</span><span class="sxs-lookup"><span data-stu-id="814ed-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="814ed-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="814ed-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-listitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="814ed-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="814ed-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-listitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="814ed-126">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="814ed-126">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="814ed-127">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="814ed-127">Default properties will be returned from the actual call.</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-create.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
