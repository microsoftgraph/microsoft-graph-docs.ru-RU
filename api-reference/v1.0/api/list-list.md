---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание списка списков SharePoint на сайте
localization_priority: Priority
ms.prod: sharepoint
description: Получение коллекции списков для сайта.
doc_type: apiPageType
ms.openlocfilehash: 060234e49943d01b1e4e992ddc41c5872ab1f775
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025542"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="02ae9-103">Перечисление списков на сайте</span><span class="sxs-lookup"><span data-stu-id="02ae9-103">Enumerate lists in a site</span></span>

<span data-ttu-id="02ae9-104">Получение коллекции [списков][] для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="02ae9-104">Get the collection of [lists][] for a [site][].</span></span>

[списков]: ../resources/list.md
[lists]: ../resources/list.md
[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="02ae9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02ae9-107">Permissions</span></span>

<span data-ttu-id="02ae9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02ae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02ae9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02ae9-110">Permission type</span></span>      | <span data-ttu-id="02ae9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02ae9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02ae9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02ae9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02ae9-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02ae9-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="02ae9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02ae9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02ae9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02ae9-115">Not supported.</span></span>    |
|<span data-ttu-id="02ae9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02ae9-116">Application</span></span> | <span data-ttu-id="02ae9-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02ae9-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02ae9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02ae9-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="02ae9-119">Пример</span><span class="sxs-lookup"><span data-stu-id="02ae9-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="02ae9-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="02ae9-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="02ae9-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="02ae9-121">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="02ae9-122">C#</span><span class="sxs-lookup"><span data-stu-id="02ae9-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02ae9-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02ae9-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02ae9-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02ae9-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="02ae9-125">Java</span><span class="sxs-lookup"><span data-stu-id="02ae9-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="02ae9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="02ae9-126">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="02ae9-127">Заметки</span><span class="sxs-lookup"><span data-stu-id="02ae9-127">Remarks</span></span>

<span data-ttu-id="02ae9-128">По умолчанию ресурсы list с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="02ae9-128">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="02ae9-129">Чтобы перечислить их, включите `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="02ae9-129">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
  ]
} -->
