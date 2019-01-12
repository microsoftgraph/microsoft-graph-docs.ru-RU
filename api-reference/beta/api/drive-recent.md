---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Создание списка последних файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d99caa91bc0b5d7140d3628db42955e558de3598
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915404"
---
# <a name="list-recent-files"></a><span data-ttu-id="189b2-102">Создание списка последних файлов</span><span class="sxs-lookup"><span data-stu-id="189b2-102">List recent files</span></span>

> <span data-ttu-id="189b2-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="189b2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="189b2-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="189b2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="189b2-p102">Указание набора элементов, которые недавно использовались пользователем, вошедшим в свою учетную запись. Эта коллекция содержит элементы, которые находятся на диске пользователя, а также элементы, к которым у него есть доступ с других дисков.</span><span class="sxs-lookup"><span data-stu-id="189b2-p102">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="189b2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="189b2-107">Permissions</span></span>

<span data-ttu-id="189b2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="189b2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="189b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="189b2-110">Permission type</span></span>      | <span data-ttu-id="189b2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="189b2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="189b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="189b2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="189b2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189b2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="189b2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="189b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="189b2-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189b2-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="189b2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="189b2-116">Application</span></span> | <span data-ttu-id="189b2-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189b2-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="189b2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="189b2-118">HTTP request</span></span>

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a><span data-ttu-id="189b2-119">Ответ</span><span class="sxs-lookup"><span data-stu-id="189b2-119">Response</span></span>

<span data-ttu-id="189b2-120">Этот метод возвращает коллекцию ресурсов [DriveItem](../resources/driveitem.md) для элементов, к которым владелец объекта drive недавно получал доступ.</span><span class="sxs-lookup"><span data-stu-id="189b2-120">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="189b2-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="189b2-121">Remarks</span></span>

<span data-ttu-id="189b2-p104">Некоторые элементы driveItem, возвращенные **последним** действием, будут содержать аспект **remoteItem**, который указывает, что это элементы с другого диска. Чтобы получить доступ к исходному объекту driveItem, следует отправить запрос, используя данные, указанные в **remoteItem** в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="189b2-p104">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files"
} -->
