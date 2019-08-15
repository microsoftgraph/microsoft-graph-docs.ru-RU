---
author: JeremyKelley
description: Создание ресурса listItem в списке.
ms.date: 09/11/2017
title: Создание записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8e584966703049edf2c650c5b0ff118d23cc8e94
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415423"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="9bbb8-103">Создание элемента в списке</span><span class="sxs-lookup"><span data-stu-id="9bbb8-103">Create a new item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bbb8-104">Создание элемента [listItem][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="9bbb8-104">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="9bbb8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9bbb8-105">Permissions</span></span>

<span data-ttu-id="9bbb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bbb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bbb8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bbb8-108">Permission type</span></span>      | <span data-ttu-id="9bbb8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bbb8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bbb8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bbb8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9bbb8-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bbb8-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9bbb8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bbb8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bbb8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bbb8-113">Not supported.</span></span>    |
|<span data-ttu-id="9bbb8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bbb8-114">Application</span></span> | <span data-ttu-id="9bbb8-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bbb8-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bbb8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bbb8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="9bbb8-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9bbb8-117">Request body</span></span>

<span data-ttu-id="9bbb8-118">В теле запроса укажите представление ресурса [listItem][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bbb8-118">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="9bbb8-119">Пример</span><span class="sxs-lookup"><span data-stu-id="9bbb8-119">Example</span></span>

<span data-ttu-id="9bbb8-120">В примере ниже показано, как создать элемент списка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="9bbb8-120">Here is an example of how to create a new generic list item.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9bbb8-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bbb8-121">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9bbb8-122">C#</span><span class="sxs-lookup"><span data-stu-id="9bbb8-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9bbb8-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bbb8-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9bbb8-124">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9bbb8-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="9bbb8-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="9bbb8-125">Response</span></span>

<span data-ttu-id="9bbb8-126">При успешном выполнении этот метод возвращает объект [listItem][] для созданного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9bbb8-126">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

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

<span data-ttu-id="9bbb8-127">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="9bbb8-127">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="9bbb8-128">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9bbb8-128">Default properties will be returned from the actual call.</span></span>

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
  ]
}
-->
