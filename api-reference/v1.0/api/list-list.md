---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание списка списков SharePoint на сайте
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d5ead524312fe1beffc561d8e936c8742c0e723a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888329"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="4f858-102">Перечисление списков на сайте</span><span class="sxs-lookup"><span data-stu-id="4f858-102">Enumerate lists in a site</span></span>

<span data-ttu-id="4f858-103">Получение коллекции [списков][] для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="4f858-103">Get the collection of [lists][] for a [site][].</span></span>

[списков]: ../resources/list.md
[lists]: ../resources/list.md
[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="4f858-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f858-106">Permissions</span></span>

<span data-ttu-id="4f858-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f858-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f858-109">Permission type</span></span>      | <span data-ttu-id="4f858-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f858-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f858-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f858-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f858-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f858-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f858-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f858-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f858-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f858-114">Not supported.</span></span>    |
|<span data-ttu-id="4f858-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f858-115">Application</span></span> | <span data-ttu-id="4f858-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f858-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f858-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f858-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="4f858-118">Пример</span><span class="sxs-lookup"><span data-stu-id="4f858-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4f858-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f858-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4f858-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f858-120">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f858-121">C#</span><span class="sxs-lookup"><span data-stu-id="4f858-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f858-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f858-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f858-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f858-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f858-124">Java</span><span class="sxs-lookup"><span data-stu-id="4f858-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f858-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f858-125">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="4f858-126">Заметки</span><span class="sxs-lookup"><span data-stu-id="4f858-126">Remarks</span></span>

<span data-ttu-id="4f858-127">По умолчанию ресурсы list с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="4f858-127">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="4f858-128">Чтобы перечислить их, включите `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="4f858-128">To list them, include `system` in your `$select` statement.</span></span>

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
