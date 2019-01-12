---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Извлечение файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 563547b5ab323f0fca4c4a8719470829e8cff22d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916161"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="1cc45-102">Получение ресурса DriveItem для изменения</span><span class="sxs-lookup"><span data-stu-id="1cc45-102">Check-out a DriveItem resource</span></span>

> <span data-ttu-id="1cc45-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1cc45-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cc45-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cc45-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1cc45-105">Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет [записан после изменения](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="1cc45-105">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc45-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1cc45-106">Permissions</span></span>

<span data-ttu-id="1cc45-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cc45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cc45-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cc45-109">Permission type</span></span>      | <span data-ttu-id="1cc45-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cc45-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cc45-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cc45-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1cc45-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cc45-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1cc45-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cc45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc45-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cc45-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1cc45-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cc45-115">Application</span></span> | <span data-ttu-id="1cc45-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cc45-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cc45-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cc45-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="1cc45-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1cc45-118">Request body</span></span>

<span data-ttu-id="1cc45-119">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="1cc45-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="1cc45-120">Пример</span><span class="sxs-lookup"><span data-stu-id="1cc45-120">Example</span></span>

<span data-ttu-id="1cc45-121">В этом примере показано, как записать после изменения файл, указанный по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="1cc45-121">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="1cc45-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cc45-122">Response</span></span>

<span data-ttu-id="1cc45-123">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="1cc45-123">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="1cc45-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="1cc45-124">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
