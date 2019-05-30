---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b788b013948d429eb5dcf726a0c9fe58af1ead81
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536339"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="c675e-102">Создание элемента в списке</span><span class="sxs-lookup"><span data-stu-id="c675e-102">Create a new item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c675e-103">Создание элемента [listItem][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="c675e-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="c675e-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c675e-104">Permissions</span></span>

<span data-ttu-id="c675e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c675e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c675e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c675e-107">Permission type</span></span>      | <span data-ttu-id="c675e-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c675e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c675e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c675e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c675e-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c675e-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c675e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c675e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c675e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c675e-112">Not supported.</span></span>    |
|<span data-ttu-id="c675e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c675e-113">Application</span></span> | <span data-ttu-id="c675e-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c675e-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c675e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c675e-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="c675e-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c675e-116">Request body</span></span>

<span data-ttu-id="c675e-117">В теле запроса укажите представление ресурса [listItem][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c675e-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="c675e-118">Пример</span><span class="sxs-lookup"><span data-stu-id="c675e-118">Example</span></span>

<span data-ttu-id="c675e-119">В примере ниже показано, как создать элемент списка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="c675e-119">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="c675e-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="c675e-120">Response</span></span>

<span data-ttu-id="c675e-121">При успешном выполнении этот метод возвращает объект [listItem][] для созданного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c675e-121">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c675e-122">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c675e-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c675e-123">C#</span><span class="sxs-lookup"><span data-stu-id="c675e-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c675e-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c675e-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-listitem-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="c675e-125">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="c675e-125">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="c675e-126">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c675e-126">Default properties will be returned from the actual call.</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/listitem-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
