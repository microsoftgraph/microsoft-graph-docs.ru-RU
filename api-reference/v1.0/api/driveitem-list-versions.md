---
title: Перечисление версий объекта DriveItem
description: OneDrive и SharePoint можно настроить на хранение журнала для файлов.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: c9fc24739f0f14a9b02cf2658794b372c9bc8393
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517708"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="be0c7-103">Перечисление версий объекта DriveItem</span><span class="sxs-lookup"><span data-stu-id="be0c7-103">Listing versions of a DriveItem</span></span>

<span data-ttu-id="be0c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be0c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="be0c7-105">OneDrive и SharePoint можно настроить на хранение журнала для файлов.</span><span class="sxs-lookup"><span data-stu-id="be0c7-105">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="be0c7-106">В зависимости от того, каковы служба и конфигурация, новую версию можно создавать при каждом изменении или сохранении, создавать вручную или не создавать никогда.</span><span class="sxs-lookup"><span data-stu-id="be0c7-106">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="be0c7-107">Предыдущие версии документа могут храниться в течение ограниченного времени в зависимости от того, каковы параметры администратора, которые могут быть уникальными для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="be0c7-107">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="be0c7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be0c7-108">Permissions</span></span>

<span data-ttu-id="be0c7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be0c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be0c7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be0c7-111">Permission type</span></span>      | <span data-ttu-id="be0c7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be0c7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be0c7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be0c7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="be0c7-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be0c7-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="be0c7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be0c7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be0c7-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be0c7-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="be0c7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be0c7-117">Application</span></span> | <span data-ttu-id="be0c7-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be0c7-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="be0c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be0c7-119">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="be0c7-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="be0c7-120">Response</span></span>

<span data-ttu-id="be0c7-121">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [DriveItemVersion](../resources/driveitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be0c7-121">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="be0c7-122">Пример</span><span class="sxs-lookup"><span data-stu-id="be0c7-122">Example</span></span>

<span data-ttu-id="be0c7-123">В этом примере показано, как получить версии файла для объекта Drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="be0c7-123">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="be0c7-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be0c7-124">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="be0c7-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="be0c7-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions
```
# <a name="c"></a>[<span data-ttu-id="be0c7-126">C#</span><span class="sxs-lookup"><span data-stu-id="be0c7-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be0c7-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be0c7-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be0c7-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be0c7-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be0c7-129">Java</span><span class="sxs-lookup"><span data-stu-id="be0c7-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be0c7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="be0c7-130">Response</span></span>

<span data-ttu-id="be0c7-131">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="be0c7-131">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="be0c7-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="be0c7-132">Remarks</span></span>

<span data-ttu-id="be0c7-133">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="be0c7-133">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="be0c7-134">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveitemversion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="be0c7-134">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
