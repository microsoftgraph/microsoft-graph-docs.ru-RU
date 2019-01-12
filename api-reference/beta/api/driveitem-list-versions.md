---
title: Список версий DriveItem
description: OneDrive и SharePoint можно настроить на хранение журнала для файлов.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 52df6b0f7e452d358160de886ed61824fd2d48d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915727"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="b34b8-103">Список версий DriveItem</span><span class="sxs-lookup"><span data-stu-id="b34b8-103">Listing versions of a DriveItem</span></span>

> <span data-ttu-id="b34b8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b34b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b34b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b34b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b34b8-106">OneDrive и SharePoint можно настроить на хранение журнала для файлов.</span><span class="sxs-lookup"><span data-stu-id="b34b8-106">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="b34b8-107">В зависимости от того, каковы служба и конфигурация, новую версию можно создавать при каждом изменении или сохранении, создавать вручную или не создавать никогда.</span><span class="sxs-lookup"><span data-stu-id="b34b8-107">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="b34b8-108">Предыдущие версии документа могут храниться в течение ограниченного времени в зависимости от того, каковы параметры администратора, которые могут быть уникальными для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="b34b8-108">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="b34b8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b34b8-109">Permissions</span></span>

<span data-ttu-id="b34b8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b34b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b34b8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b34b8-112">Permission type</span></span>      | <span data-ttu-id="b34b8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b34b8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b34b8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b34b8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b34b8-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b34b8-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b34b8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b34b8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b34b8-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b34b8-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b34b8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b34b8-118">Application</span></span> | <span data-ttu-id="b34b8-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b34b8-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="b34b8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b34b8-120">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="b34b8-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="b34b8-121">Response</span></span>

<span data-ttu-id="b34b8-122">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [DriveItemVersion](../resources/driveitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b34b8-122">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="b34b8-123">Пример</span><span class="sxs-lookup"><span data-stu-id="b34b8-123">Example</span></span>

<span data-ttu-id="b34b8-124">В этом примере показано, как получить версии файла для объекта Drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="b34b8-124">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="b34b8-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b34b8-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="b34b8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b34b8-126">Response</span></span>

<span data-ttu-id="b34b8-127">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="b34b8-127">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

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
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="b34b8-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="b34b8-128">Remarks</span></span>

<span data-ttu-id="b34b8-129">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="b34b8-129">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="b34b8-130">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveitemversion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="b34b8-130">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
