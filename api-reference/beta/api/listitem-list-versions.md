---
author: JeremyKelley
description: Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.
ms.date: 09/10/2017
title: Получение предыдущей версии записи списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: cf3d0a88f250a954e5143c1000bcf4aaf61c0c1e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993069"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="261f7-103">Создание списка версий элемента ListItem (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="261f7-103">Listing versions of a ListItem (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="261f7-104">Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.</span><span class="sxs-lookup"><span data-stu-id="261f7-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="261f7-105">Предыдущие версии можно хранить в течение конечного периода времени, настроенного администратором. Такой период можно задавать отдельно для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="261f7-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="261f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="261f7-106">Permissions</span></span>

<span data-ttu-id="261f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="261f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="261f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="261f7-109">Permission type</span></span>             | <span data-ttu-id="261f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="261f7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="261f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="261f7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="261f7-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="261f7-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="261f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="261f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="261f7-114">Н/д</span><span class="sxs-lookup"><span data-stu-id="261f7-114">n/a</span></span>                                         |
| <span data-ttu-id="261f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="261f7-115">Application</span></span>                            | <span data-ttu-id="261f7-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="261f7-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="261f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="261f7-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="261f7-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="261f7-118">Response</span></span>

<span data-ttu-id="261f7-119">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="261f7-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="261f7-120">Пример</span><span class="sxs-lookup"><span data-stu-id="261f7-120">Example</span></span>

<span data-ttu-id="261f7-121">В этом примере показано, как получить версии элемента listItem в списке SharePoint:</span><span class="sxs-lookup"><span data-stu-id="261f7-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="261f7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="261f7-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="261f7-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="261f7-123">Response</span></span>

<span data-ttu-id="261f7-124">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="261f7-124">This returns a collection of versions:</span></span>

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


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": []
}
-->
