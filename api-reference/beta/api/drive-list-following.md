---
author: chackman
description: Список элементов, за которыми подписан пользователь, вошедшего в систему.
title: Список отслеживаемых элементов
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 20c5d9801480799503e2ac6cdcefca64daae4a5d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955876"
---
# <a name="list-followed-items"></a><span data-ttu-id="ed18c-103">Список отслеживаемых элементов</span><span class="sxs-lookup"><span data-stu-id="ed18c-103">List followed items</span></span>

<span data-ttu-id="ed18c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed18c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed18c-105">Список [элементов](../resources/driveitem.md) , за которыми подписан пользователь, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="ed18c-105">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="ed18c-106">Эта коллекция содержит элементы, которые находятся на диске пользователя, а также элементы, к которым у него есть доступ с других дисков.</span><span class="sxs-lookup"><span data-stu-id="ed18c-106">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed18c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed18c-107">Permissions</span></span>

<span data-ttu-id="ed18c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed18c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed18c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed18c-110">Permission type</span></span>      | <span data-ttu-id="ed18c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed18c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed18c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed18c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ed18c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed18c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed18c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed18c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed18c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed18c-115">Not supported.</span></span>    |
|<span data-ttu-id="ed18c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed18c-116">Application</span></span> | <span data-ttu-id="ed18c-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed18c-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed18c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed18c-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="ed18c-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed18c-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/following
```
# <a name="c"></a>[<span data-ttu-id="ed18c-120">C#</span><span class="sxs-lookup"><span data-stu-id="ed18c-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-followed-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed18c-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed18c-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-followed-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed18c-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed18c-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-followed-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed18c-123">Java</span><span class="sxs-lookup"><span data-stu-id="ed18c-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-followed-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="ed18c-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed18c-124">Response</span></span>

<span data-ttu-id="ed18c-125">Этот метод возвращает коллекцию ресурсов [driveItem](../resources/driveitem.md) для элементов, которые подписаны владельцем диска.</span><span class="sxs-lookup"><span data-stu-id="ed18c-125">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="ed18c-126">Если не будет найдено ни одного элемента, то будет возвращена пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="ed18c-126">If no items were found, an empty collection is returned.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
  ]
}
-->


