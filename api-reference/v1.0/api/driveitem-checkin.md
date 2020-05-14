---
author: learafa
description: Возврат извлеченного ресурса driveItem, который делает версию документа доступной другим пользователям.
title: 'driveItem: checkin'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 7cf999dc338c4a16a4040e8b48b4824c6da09e94
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43511135"
---
# <a name="driveitem-checkin"></a><span data-ttu-id="60bf6-103">driveItem: checkin</span><span class="sxs-lookup"><span data-stu-id="60bf6-103">driveItem: checkin</span></span>

<span data-ttu-id="60bf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60bf6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60bf6-105">Возврат извлеченного ресурса **driveItem** , который делает версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="60bf6-105">Check in a checked out **driveItem** resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="60bf6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60bf6-106">Permissions</span></span>

<span data-ttu-id="60bf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60bf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60bf6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60bf6-109">Permission type</span></span>      | <span data-ttu-id="60bf6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60bf6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60bf6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60bf6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="60bf6-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60bf6-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="60bf6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60bf6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60bf6-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60bf6-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="60bf6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60bf6-115">Application</span></span> | <span data-ttu-id="60bf6-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60bf6-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60bf6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60bf6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

## <a name="request-body"></a><span data-ttu-id="60bf6-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60bf6-118">Request body</span></span>

<span data-ttu-id="60bf6-119">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="60bf6-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="60bf6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="60bf6-120">Name</span></span>    | <span data-ttu-id="60bf6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="60bf6-121">Value</span></span>  |                                                <span data-ttu-id="60bf6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="60bf6-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="60bf6-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="60bf6-123">checkInAs</span></span> | <span data-ttu-id="60bf6-124">string</span><span class="sxs-lookup"><span data-stu-id="60bf6-124">string</span></span> | <span data-ttu-id="60bf6-125">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="60bf6-125">Optional.</span></span> <span data-ttu-id="60bf6-126">Состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="60bf6-126">The status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="60bf6-127">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="60bf6-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="60bf6-128">comment</span><span class="sxs-lookup"><span data-stu-id="60bf6-128">comment</span></span>   | <span data-ttu-id="60bf6-129">string</span><span class="sxs-lookup"><span data-stu-id="60bf6-129">string</span></span> | <span data-ttu-id="60bf6-130">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="60bf6-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="response"></a><span data-ttu-id="60bf6-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="60bf6-131">Response</span></span>

<span data-ttu-id="60bf6-132">В случае успеха вызов API возвращает `204 No content` .</span><span class="sxs-lookup"><span data-stu-id="60bf6-132">If successful, the API call returns `204 No content`.</span></span>

## <a name="example"></a><span data-ttu-id="60bf6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="60bf6-133">Example</span></span>

<span data-ttu-id="60bf6-134">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="60bf6-134">This example checks in a file identified by `{item-id}`.</span></span>

### <a name="request"></a><span data-ttu-id="60bf6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="60bf6-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="60bf6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="60bf6-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="c"></a>[<span data-ttu-id="60bf6-137">C#</span><span class="sxs-lookup"><span data-stu-id="60bf6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60bf6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60bf6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60bf6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60bf6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60bf6-140">Java</span><span class="sxs-lookup"><span data-stu-id="60bf6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkin-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60bf6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="60bf6-141">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
