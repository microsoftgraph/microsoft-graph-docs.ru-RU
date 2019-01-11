---
title: Получение ListItemVersion ресурсов
description: В этой статье рассказывается, как получить метаданные для определенной версии ресурса ListItem.
localization_priority: Normal
ms.openlocfilehash: 54fb491a13e90e1133127531d32c29e1ec2fa040
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888230"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="24f97-103">Получение ListItemVersion ресурсов</span><span class="sxs-lookup"><span data-stu-id="24f97-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="24f97-104">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="24f97-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="24f97-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24f97-105">Permissions</span></span>

<span data-ttu-id="24f97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24f97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="24f97-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24f97-108">Permission type</span></span>             | <span data-ttu-id="24f97-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24f97-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="24f97-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24f97-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="24f97-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24f97-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="24f97-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24f97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24f97-113">Н/д</span><span class="sxs-lookup"><span data-stu-id="24f97-113">n/a</span></span>                                         |
| <span data-ttu-id="24f97-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24f97-114">Application</span></span>                            | <span data-ttu-id="24f97-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24f97-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="24f97-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24f97-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="24f97-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="24f97-117">Response</span></span>

<span data-ttu-id="24f97-118">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [ListItemVersion](../resources/listitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="24f97-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="24f97-119">Пример</span><span class="sxs-lookup"><span data-stu-id="24f97-119">Example</span></span>

<span data-ttu-id="24f97-120">В этом примере показано, как получить версию объекта listItem и расширить коллекцию полей для запроса значений полей в объекте listItem.</span><span class="sxs-lookup"><span data-stu-id="24f97-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="24f97-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24f97-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="24f97-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="24f97-122">Response</span></span>

<span data-ttu-id="24f97-123">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="24f97-123">This returns a collection of versions:</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
