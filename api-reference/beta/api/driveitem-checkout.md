---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Извлечение файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5da9dba96ca19d94bd0eec8a8039e752ec28b894
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325366"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="30701-102">Получение ресурса DriveItem для изменения</span><span class="sxs-lookup"><span data-stu-id="30701-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30701-103">Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет [записан после изменения](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="30701-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="30701-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30701-104">Permissions</span></span>

<span data-ttu-id="30701-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30701-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30701-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30701-107">Permission type</span></span>      | <span data-ttu-id="30701-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30701-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30701-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30701-109">Delegated (work or school account)</span></span> | <span data-ttu-id="30701-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30701-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="30701-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30701-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30701-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30701-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="30701-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30701-113">Application</span></span> | <span data-ttu-id="30701-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30701-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30701-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30701-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="30701-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30701-116">Request body</span></span>

<span data-ttu-id="30701-117">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="30701-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="30701-118">Пример</span><span class="sxs-lookup"><span data-stu-id="30701-118">Example</span></span>

<span data-ttu-id="30701-119">В этом примере показано, как записать после изменения файл, указанный по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="30701-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="30701-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="30701-120">Response</span></span>

<span data-ttu-id="30701-121">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="30701-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="30701-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="30701-122">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": []
}
-->
