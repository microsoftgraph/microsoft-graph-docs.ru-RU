---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание записи в списке SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 80d401f45c5a43428239e6473e9acd44a8466d8e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459001"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="f188e-102">Создание элемента в списке</span><span class="sxs-lookup"><span data-stu-id="f188e-102">Create a new item in a list</span></span>

<span data-ttu-id="f188e-103">Создание элемента [listItem][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="f188e-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="f188e-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f188e-104">Permissions</span></span>

<span data-ttu-id="f188e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f188e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f188e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f188e-107">Permission type</span></span>      | <span data-ttu-id="f188e-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f188e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f188e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f188e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f188e-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f188e-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f188e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f188e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f188e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f188e-112">Not supported.</span></span>    |
|<span data-ttu-id="f188e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f188e-113">Application</span></span> | <span data-ttu-id="f188e-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f188e-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f188e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f188e-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="f188e-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f188e-116">Request body</span></span>

<span data-ttu-id="f188e-117">В теле запроса укажите представление ресурса [listItem][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f188e-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="f188e-118">Пример</span><span class="sxs-lookup"><span data-stu-id="f188e-118">Example</span></span>

<span data-ttu-id="f188e-119">В примере ниже показано, как создать элемент списка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="f188e-119">Here is an example of how to create a new generic list item.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f188e-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="f188e-120">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f188e-121">C#</span><span class="sxs-lookup"><span data-stu-id="f188e-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f188e-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f188e-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f188e-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f188e-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="f188e-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="f188e-124">Response</span></span>

<span data-ttu-id="f188e-125">При успешном выполнении этот метод возвращает объект [listItem][] для созданного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f188e-125">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

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

<span data-ttu-id="f188e-126">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="f188e-126">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="f188e-127">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f188e-127">Default properties will be returned from the actual call.</span></span>

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
