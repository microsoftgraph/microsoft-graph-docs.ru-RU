---
title: Перечисление версий элемента ListItem
description: Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 3edbd65ce3201b3595215f221fa5616a194306d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057264"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="ee849-103">Перечисление версий элемента ListItem</span><span class="sxs-lookup"><span data-stu-id="ee849-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="ee849-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee849-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee849-105">Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.</span><span class="sxs-lookup"><span data-stu-id="ee849-105">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="ee849-106">Предыдущие версии можно хранить в течение конечного периода времени, настроенного администратором. Такой период можно задавать отдельно для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="ee849-106">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee849-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee849-107">Permissions</span></span>

<span data-ttu-id="ee849-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="ee849-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee849-110">Permission type</span></span>             | <span data-ttu-id="ee849-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee849-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ee849-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee849-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee849-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee849-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="ee849-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee849-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee849-115">Н/д</span><span class="sxs-lookup"><span data-stu-id="ee849-115">n/a</span></span>                                         |
| <span data-ttu-id="ee849-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee849-116">Application</span></span>                            | <span data-ttu-id="ee849-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee849-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="ee849-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee849-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="ee849-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee849-119">Response</span></span>

<span data-ttu-id="ee849-120">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ee849-120">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="ee849-121">Пример</span><span class="sxs-lookup"><span data-stu-id="ee849-121">Example</span></span>

<span data-ttu-id="ee849-122">В этом примере показано, как получить версии элемента listItem в списке SharePoint:</span><span class="sxs-lookup"><span data-stu-id="ee849-122">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="ee849-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee849-123">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="ee849-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee849-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```
# <a name="c"></a>[<span data-ttu-id="ee849-125">C#</span><span class="sxs-lookup"><span data-stu-id="ee849-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee849-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee849-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee849-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee849-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee849-128">Java</span><span class="sxs-lookup"><span data-stu-id="ee849-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee849-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee849-129">Response</span></span>

<span data-ttu-id="ee849-130">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="ee849-130">This returns a collection of versions:</span></span>

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

