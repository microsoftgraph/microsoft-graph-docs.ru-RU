---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Возврат файлов
localization_priority: Normal
ms.openlocfilehash: 685bd89ed13bba4c4687620b00d346c7557214c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853930"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="2d44e-102">Возврат изменений в ресурсе DriveItem</span><span class="sxs-lookup"><span data-stu-id="2d44e-102">Check-in changes to a DriveItem resource</span></span>

> <span data-ttu-id="2d44e-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2d44e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d44e-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d44e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d44e-105">В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="2d44e-105">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d44e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d44e-106">Permissions</span></span>

<span data-ttu-id="2d44e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d44e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d44e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d44e-109">Permission type</span></span>      | <span data-ttu-id="2d44e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d44e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d44e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d44e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d44e-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d44e-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d44e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d44e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d44e-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d44e-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d44e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d44e-115">Application</span></span> | <span data-ttu-id="2d44e-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d44e-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d44e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d44e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="2d44e-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d44e-118">Request body</span></span>

<span data-ttu-id="2d44e-119">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2d44e-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="2d44e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2d44e-120">Name</span></span>    | <span data-ttu-id="2d44e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2d44e-121">Value</span></span>  |                                                <span data-ttu-id="2d44e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2d44e-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2d44e-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="2d44e-123">checkInAs</span></span> | <span data-ttu-id="2d44e-124">string</span><span class="sxs-lookup"><span data-stu-id="2d44e-124">string</span></span> | <span data-ttu-id="2d44e-125">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2d44e-125">Optional.</span></span> <span data-ttu-id="2d44e-126">Желаемое состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="2d44e-126">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="2d44e-127">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="2d44e-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="2d44e-128">comment</span><span class="sxs-lookup"><span data-stu-id="2d44e-128">comment</span></span>   | <span data-ttu-id="2d44e-129">строка</span><span class="sxs-lookup"><span data-stu-id="2d44e-129">string</span></span> | <span data-ttu-id="2d44e-130">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="2d44e-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="2d44e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2d44e-131">Example</span></span>

<span data-ttu-id="2d44e-132">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="2d44e-132">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="2d44e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d44e-133">Response</span></span>

<span data-ttu-id="2d44e-134">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="2d44e-134">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="2d44e-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="2d44e-135">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
