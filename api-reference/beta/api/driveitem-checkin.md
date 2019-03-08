---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Возврат файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ea8d4b8ec5399e867bd94c261ce95783f8ea27ba
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481078"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="16a87-102">Возврат изменений в ресурсе DriveItem</span><span class="sxs-lookup"><span data-stu-id="16a87-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16a87-103">В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="16a87-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="16a87-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16a87-104">Permissions</span></span>

<span data-ttu-id="16a87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16a87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16a87-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16a87-107">Permission type</span></span>      | <span data-ttu-id="16a87-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16a87-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16a87-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16a87-109">Delegated (work or school account)</span></span> | <span data-ttu-id="16a87-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16a87-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="16a87-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16a87-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16a87-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16a87-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="16a87-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16a87-113">Application</span></span> | <span data-ttu-id="16a87-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16a87-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16a87-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16a87-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="16a87-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16a87-116">Request body</span></span>

<span data-ttu-id="16a87-117">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="16a87-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="16a87-118">Имя</span><span class="sxs-lookup"><span data-stu-id="16a87-118">Name</span></span>    | <span data-ttu-id="16a87-119">Значение</span><span class="sxs-lookup"><span data-stu-id="16a87-119">Value</span></span>  |                                                <span data-ttu-id="16a87-120">Описание</span><span class="sxs-lookup"><span data-stu-id="16a87-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="16a87-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="16a87-121">checkInAs</span></span> | <span data-ttu-id="16a87-122">string</span><span class="sxs-lookup"><span data-stu-id="16a87-122">string</span></span> | <span data-ttu-id="16a87-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="16a87-123">Optional.</span></span> <span data-ttu-id="16a87-124">Желаемое состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="16a87-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="16a87-125">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="16a87-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="16a87-126">comment</span><span class="sxs-lookup"><span data-stu-id="16a87-126">comment</span></span>   | <span data-ttu-id="16a87-127">string</span><span class="sxs-lookup"><span data-stu-id="16a87-127">string</span></span> | <span data-ttu-id="16a87-128">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="16a87-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="16a87-129">Пример</span><span class="sxs-lookup"><span data-stu-id="16a87-129">Example</span></span>

<span data-ttu-id="16a87-130">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="16a87-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="16a87-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="16a87-131">Response</span></span>

<span data-ttu-id="16a87-132">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="16a87-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="16a87-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="16a87-133">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
