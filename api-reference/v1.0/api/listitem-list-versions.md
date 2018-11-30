---
title: Список версий элемента управления ListItem
description: Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.
ms.openlocfilehash: 43f28b355b733ba9651bba90f81179e59ebd3610
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025856"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="decdc-103">Список версий элемента управления ListItem</span><span class="sxs-lookup"><span data-stu-id="decdc-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="decdc-104">Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.</span><span class="sxs-lookup"><span data-stu-id="decdc-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="decdc-105">Предыдущие версии можно хранить в течение конечного периода времени, настроенного администратором. Такой период можно задавать отдельно для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="decdc-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="decdc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="decdc-106">Permissions</span></span>

<span data-ttu-id="decdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="decdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="decdc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="decdc-109">Permission type</span></span>             | <span data-ttu-id="decdc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="decdc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="decdc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="decdc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="decdc-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="decdc-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="decdc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="decdc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="decdc-114">Н/д</span><span class="sxs-lookup"><span data-stu-id="decdc-114">n/a</span></span>                                         |
| <span data-ttu-id="decdc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="decdc-115">Application</span></span>                            | <span data-ttu-id="decdc-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="decdc-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="decdc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="decdc-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="decdc-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="decdc-118">Response</span></span>

<span data-ttu-id="decdc-119">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="decdc-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="decdc-120">Пример</span><span class="sxs-lookup"><span data-stu-id="decdc-120">Example</span></span>

<span data-ttu-id="decdc-121">В этом примере показано, как получить версии элемента listItem в списке SharePoint:</span><span class="sxs-lookup"><span data-stu-id="decdc-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="decdc-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="decdc-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="decdc-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="decdc-123">Response</span></span>

<span data-ttu-id="decdc-124">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="decdc-124">This returns a collection of versions:</span></span>

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
  "tocPath": "Items/Version history"
} -->
