---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Получение предыдущей версии записи списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2b79205da64a254c1d09cdaff8ae1ba153ec9ce9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528839"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="17517-102">Создание списка версий элемента ListItem (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="17517-102">Listing versions of a ListItem (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17517-103">Вы можете настроить SharePoint так, чтобы в нем хранился журнал элементов списка.</span><span class="sxs-lookup"><span data-stu-id="17517-103">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="17517-104">Предыдущие версии можно хранить в течение конечного периода времени, настроенного администратором. Такой период можно задавать отдельно для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="17517-104">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="17517-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17517-105">Permissions</span></span>

<span data-ttu-id="17517-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17517-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="17517-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17517-108">Permission type</span></span>             | <span data-ttu-id="17517-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17517-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="17517-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17517-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="17517-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17517-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="17517-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17517-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17517-113">Н/д</span><span class="sxs-lookup"><span data-stu-id="17517-113">n/a</span></span>                                         |
| <span data-ttu-id="17517-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17517-114">Application</span></span>                            | <span data-ttu-id="17517-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17517-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="17517-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17517-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="17517-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="17517-117">Response</span></span>

<span data-ttu-id="17517-118">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="17517-118">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="17517-119">Пример</span><span class="sxs-lookup"><span data-stu-id="17517-119">Example</span></span>

<span data-ttu-id="17517-120">В этом примере показано, как получить версии элемента listItem в списке SharePoint:</span><span class="sxs-lookup"><span data-stu-id="17517-120">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="17517-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17517-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="17517-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="17517-122">Response</span></span>

<span data-ttu-id="17517-123">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="17517-123">This returns a collection of versions:</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-list-versions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
