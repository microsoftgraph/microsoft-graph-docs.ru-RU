---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание записи в списке SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 3037903ae448fc4d05b0c8478e78ccb573aeb588
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880741"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="1857b-102">Создание элемента в списке</span><span class="sxs-lookup"><span data-stu-id="1857b-102">Create a new item in a list</span></span>

<span data-ttu-id="1857b-103">Создание элемента [listItem][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="1857b-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="1857b-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1857b-104">Permissions</span></span>

<span data-ttu-id="1857b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1857b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1857b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1857b-107">Permission type</span></span>      | <span data-ttu-id="1857b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1857b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1857b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1857b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1857b-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1857b-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1857b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1857b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1857b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1857b-112">Not supported.</span></span>    |
|<span data-ttu-id="1857b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1857b-113">Application</span></span> | <span data-ttu-id="1857b-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1857b-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1857b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1857b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="1857b-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1857b-116">Request body</span></span>

<span data-ttu-id="1857b-117">В теле запроса укажите представление ресурса [listItem][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1857b-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="1857b-118">Пример</span><span class="sxs-lookup"><span data-stu-id="1857b-118">Example</span></span>

<span data-ttu-id="1857b-119">В примере ниже показано, как создать элемент списка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="1857b-119">Here is an example of how to create a new generic list item.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1857b-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="1857b-120">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1857b-121">C#</span><span class="sxs-lookup"><span data-stu-id="1857b-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1857b-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1857b-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1857b-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1857b-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1857b-124">Java</span><span class="sxs-lookup"><span data-stu-id="1857b-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="1857b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1857b-125">Response</span></span>

<span data-ttu-id="1857b-126">При успешном выполнении этот метод возвращает объект [listItem][] для созданного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1857b-126">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

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

<span data-ttu-id="1857b-127">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="1857b-127">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="1857b-128">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1857b-128">Default properties will be returned from the actual call.</span></span>

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
  ]
} -->
