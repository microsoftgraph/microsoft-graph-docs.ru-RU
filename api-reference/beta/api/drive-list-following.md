---
author: chackman
ms.author: chackman
title: Число элементов списка
ms.openlocfilehash: dfaa727d25b3713d1be2a8d49f87dab8dba3b553
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079718"
---
# <a name="list-followed-items"></a><span data-ttu-id="8eb41-102">Число элементов списка</span><span class="sxs-lookup"><span data-stu-id="8eb41-102">List followed items</span></span>

> <span data-ttu-id="8eb41-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8eb41-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eb41-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb41-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eb41-105">Список [элементов](../resources/driveitem.md) , следуют выполнен вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="8eb41-105">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="8eb41-106">Данная коллекция включает элементов, находящихся в диске компьютера пользователя, а также элементы, которые получают доступ из других дисков.</span><span class="sxs-lookup"><span data-stu-id="8eb41-106">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="8eb41-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8eb41-107">Permissions</span></span>

<span data-ttu-id="8eb41-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eb41-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eb41-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8eb41-110">Permission type</span></span>      | <span data-ttu-id="8eb41-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8eb41-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eb41-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8eb41-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8eb41-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb41-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8eb41-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8eb41-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eb41-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb41-115">Not supported.</span></span>    |
|<span data-ttu-id="8eb41-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8eb41-116">Application</span></span> | <span data-ttu-id="8eb41-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb41-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8eb41-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eb41-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="8eb41-119">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eb41-119">Response</span></span>

<span data-ttu-id="8eb41-120">Этот метод возвращает коллекцию ресурсов [driveItem](../resources/driveitem.md) для элементов, которые выполнив владельца диска.</span><span class="sxs-lookup"><span data-stu-id="8eb41-120">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="8eb41-121">Если не найдено элементов, возвращается пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="8eb41-121">If no items were found, an empty collection is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items"
} -->
