---
author: JeremyKelley
description: Указание набора элементов, которые недавно использовались пользователем, вошедшим в свою учетную запись.
ms.date: 09/10/2017
title: Список последних файлов
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 40ea44221359d47f8290b34538b62763a2070e12
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433141"
---
# <a name="list-recent-files"></a><span data-ttu-id="653e6-103">Список последних файлов</span><span class="sxs-lookup"><span data-stu-id="653e6-103">List recent files</span></span>

<span data-ttu-id="653e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="653e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="653e6-p101">Указание набора элементов, которые недавно использовались пользователем, вошедшим в свою учетную запись. Эта коллекция содержит элементы, которые находятся на диске пользователя, а также элементы, к которым у него есть доступ с других дисков.</span><span class="sxs-lookup"><span data-stu-id="653e6-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="653e6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="653e6-107">Permissions</span></span>

<span data-ttu-id="653e6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="653e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="653e6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="653e6-110">Permission type</span></span>      | <span data-ttu-id="653e6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="653e6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="653e6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="653e6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="653e6-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="653e6-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="653e6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="653e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="653e6-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="653e6-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="653e6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="653e6-116">Application</span></span> | <span data-ttu-id="653e6-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="653e6-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="653e6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="653e6-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="653e6-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="653e6-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "target": "action" } -->

```msgraph-interactive
GET /me/drive/recent
```
# <a name="c"></a>[<span data-ttu-id="653e6-120">C#</span><span class="sxs-lookup"><span data-stu-id="653e6-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/view-recent-files-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="653e6-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="653e6-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/view-recent-files-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="653e6-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="653e6-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/view-recent-files-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="653e6-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="653e6-123">Response</span></span>

<span data-ttu-id="653e6-124">Этот метод возвращает коллекцию ресурсов [DriveItem](../resources/driveitem.md) для элементов, к которым владелец объекта drive недавно получал доступ.</span><span class="sxs-lookup"><span data-stu-id="653e6-124">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

<!-- { "blockType": "response",
       "@odata.type": "Collection(microsoft.graph.driveItem)",
       "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T19:13:00Z"
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T16:43:21Z"
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="653e6-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="653e6-125">Remarks</span></span>

<span data-ttu-id="653e6-p103">Некоторые элементы driveItem, возвращенные **последним** действием, будут содержать аспект **remoteItem**, который указывает, что это элементы с другого диска. Чтобы получить доступ к исходному объекту driveItem, следует отправить запрос, используя данные, указанные в **remoteItem** в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="653e6-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files",
  "suppressions": [
  ]
}
-->
