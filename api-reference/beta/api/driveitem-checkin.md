---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Возврат файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fb62dc05c60e26a6d1d6683913eeec0403d1c41c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950811"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="152e9-102">Возврат изменений в ресурсе DriveItem</span><span class="sxs-lookup"><span data-stu-id="152e9-102">Check-in changes to a DriveItem resource</span></span>

> <span data-ttu-id="152e9-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="152e9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="152e9-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="152e9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="152e9-105">В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="152e9-105">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="152e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="152e9-106">Permissions</span></span>

<span data-ttu-id="152e9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="152e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="152e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="152e9-109">Permission type</span></span>      | <span data-ttu-id="152e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="152e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="152e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="152e9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="152e9-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="152e9-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="152e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="152e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="152e9-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="152e9-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="152e9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="152e9-115">Application</span></span> | <span data-ttu-id="152e9-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="152e9-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="152e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="152e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="152e9-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="152e9-118">Request body</span></span>

<span data-ttu-id="152e9-119">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="152e9-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="152e9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="152e9-120">Name</span></span>    | <span data-ttu-id="152e9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="152e9-121">Value</span></span>  |                                                <span data-ttu-id="152e9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="152e9-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="152e9-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="152e9-123">checkInAs</span></span> | <span data-ttu-id="152e9-124">string</span><span class="sxs-lookup"><span data-stu-id="152e9-124">string</span></span> | <span data-ttu-id="152e9-125">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="152e9-125">Optional.</span></span> <span data-ttu-id="152e9-126">Желаемое состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="152e9-126">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="152e9-127">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="152e9-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="152e9-128">comment</span><span class="sxs-lookup"><span data-stu-id="152e9-128">comment</span></span>   | <span data-ttu-id="152e9-129">строка</span><span class="sxs-lookup"><span data-stu-id="152e9-129">string</span></span> | <span data-ttu-id="152e9-130">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="152e9-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="152e9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="152e9-131">Example</span></span>

<span data-ttu-id="152e9-132">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="152e9-132">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="152e9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="152e9-133">Response</span></span>

<span data-ttu-id="152e9-134">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="152e9-134">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="152e9-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="152e9-135">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
