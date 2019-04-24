---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Извлечение файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bd69a02a3c243a86d7f9d05b54eb3fac00eeee88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454731"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="ef52b-102">Получение ресурса DriveItem для изменения</span><span class="sxs-lookup"><span data-stu-id="ef52b-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef52b-103">Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет [записан после изменения](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="ef52b-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef52b-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef52b-104">Permissions</span></span>

<span data-ttu-id="ef52b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef52b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef52b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef52b-107">Permission type</span></span>      | <span data-ttu-id="ef52b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef52b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef52b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef52b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ef52b-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef52b-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef52b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef52b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef52b-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef52b-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef52b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef52b-113">Application</span></span> | <span data-ttu-id="ef52b-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef52b-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef52b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef52b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="ef52b-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef52b-116">Request body</span></span>

<span data-ttu-id="ef52b-117">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="ef52b-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="ef52b-118">Пример</span><span class="sxs-lookup"><span data-stu-id="ef52b-118">Example</span></span>

<span data-ttu-id="ef52b-119">В этом примере показано, как записать после изменения файл, указанный по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="ef52b-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="ef52b-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef52b-120">Response</span></span>

<span data-ttu-id="ef52b-121">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="ef52b-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="ef52b-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="ef52b-122">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
