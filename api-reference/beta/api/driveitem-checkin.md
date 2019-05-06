---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Возврат файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 982a581d44e39e6ddcc7bb3a52da64cd2a2eaf55
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589368"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="b4748-102">Возврат изменений в ресурсе DriveItem</span><span class="sxs-lookup"><span data-stu-id="b4748-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4748-103">В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="b4748-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4748-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4748-104">Permissions</span></span>

<span data-ttu-id="b4748-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4748-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4748-107">Permission type</span></span>      | <span data-ttu-id="b4748-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4748-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4748-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4748-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b4748-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4748-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4748-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4748-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4748-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4748-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4748-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4748-113">Application</span></span> | <span data-ttu-id="b4748-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4748-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4748-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4748-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="b4748-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4748-116">Request body</span></span>

<span data-ttu-id="b4748-117">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b4748-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="b4748-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b4748-118">Name</span></span>    | <span data-ttu-id="b4748-119">Значение</span><span class="sxs-lookup"><span data-stu-id="b4748-119">Value</span></span>  |                                                <span data-ttu-id="b4748-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b4748-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b4748-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="b4748-121">checkInAs</span></span> | <span data-ttu-id="b4748-122">string</span><span class="sxs-lookup"><span data-stu-id="b4748-122">string</span></span> | <span data-ttu-id="b4748-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b4748-123">Optional.</span></span> <span data-ttu-id="b4748-124">Желаемое состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="b4748-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="b4748-125">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="b4748-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="b4748-126">comment</span><span class="sxs-lookup"><span data-stu-id="b4748-126">comment</span></span>   | <span data-ttu-id="b4748-127">string</span><span class="sxs-lookup"><span data-stu-id="b4748-127">string</span></span> | <span data-ttu-id="b4748-128">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="b4748-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="b4748-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b4748-129">Example</span></span>

<span data-ttu-id="b4748-130">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="b4748-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="b4748-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4748-131">Response</span></span>

<span data-ttu-id="b4748-132">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="b4748-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b4748-133">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="b4748-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b4748-134">Языках</span><span class="sxs-lookup"><span data-stu-id="b4748-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/checkin-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4748-135">Язык</span><span class="sxs-lookup"><span data-stu-id="b4748-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/checkin-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="remarks"></a><span data-ttu-id="b4748-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="b4748-136">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-checkin.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
