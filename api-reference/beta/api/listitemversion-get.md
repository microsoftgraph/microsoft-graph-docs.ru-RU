---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 'Получение предыдущей версии элемента списка: API SharePoint'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a23a8218b2be3ff36d719ee25e6fb0c960c5750f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526258"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="5b93b-102">Получение ресурса ListItemVersion (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="5b93b-102">Get a ListItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b93b-103">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="5b93b-103">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b93b-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b93b-104">Permissions</span></span>

<span data-ttu-id="5b93b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b93b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="5b93b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b93b-107">Permission type</span></span>             | <span data-ttu-id="5b93b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b93b-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5b93b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b93b-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b93b-110">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b93b-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="5b93b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b93b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b93b-112">Н/д</span><span class="sxs-lookup"><span data-stu-id="5b93b-112">n/a</span></span>                                         |
| <span data-ttu-id="5b93b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b93b-113">Application</span></span>                            | <span data-ttu-id="5b93b-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b93b-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="5b93b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b93b-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="5b93b-116">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b93b-116">Response</span></span>

<span data-ttu-id="5b93b-117">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5b93b-117">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="5b93b-118">Пример</span><span class="sxs-lookup"><span data-stu-id="5b93b-118">Example</span></span>

<span data-ttu-id="5b93b-119">В этом примере показано, как получить версию объекта listItem и расширить коллекцию полей для запроса значений полей в объекте listItem.</span><span class="sxs-lookup"><span data-stu-id="5b93b-119">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="5b93b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b93b-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="5b93b-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b93b-121">Response</span></span>

<span data-ttu-id="5b93b-122">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="5b93b-122">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
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
    "Error: /api-reference/beta/api/listitemversion-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
