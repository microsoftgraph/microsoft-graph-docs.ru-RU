---
author: chackman
ms.author: chackman
title: Следуйте элемента диска
localization_priority: Normal
ms.openlocfilehash: 5ba37773f552015b6c762b2b10d801b40670a03c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875035"
---
# <a name="follow-drive-item"></a><span data-ttu-id="eba0b-102">Следуйте элемента диска</span><span class="sxs-lookup"><span data-stu-id="eba0b-102">Follow drive item</span></span>

> <span data-ttu-id="eba0b-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eba0b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eba0b-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eba0b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eba0b-105">Следуйте [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="eba0b-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="eba0b-106">**Примечание:** Чтобы отменить подписку на элемент, обратитесь к [Unfollow элемента](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="eba0b-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eba0b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eba0b-107">Permissions</span></span>

<span data-ttu-id="eba0b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eba0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eba0b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eba0b-110">Permission type</span></span>      | <span data-ttu-id="eba0b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eba0b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eba0b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eba0b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eba0b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba0b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eba0b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eba0b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eba0b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eba0b-115">Not supported.</span></span>    |
|<span data-ttu-id="eba0b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eba0b-116">Application</span></span> | <span data-ttu-id="eba0b-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba0b-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eba0b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eba0b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="eba0b-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eba0b-119">Request body</span></span>

<span data-ttu-id="eba0b-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="eba0b-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="eba0b-121">Ответ</span><span class="sxs-lookup"><span data-stu-id="eba0b-121">Response</span></span>

<span data-ttu-id="eba0b-122">Этот метод возвращает [DriveItem](../resources/driveitem.md) для элемента а затем.</span><span class="sxs-lookup"><span data-stu-id="eba0b-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="eba0b-123">Пример</span><span class="sxs-lookup"><span data-stu-id="eba0b-123">Example</span></span>

<span data-ttu-id="eba0b-124">В этом примере исходя из элемента, определяемую средством `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="eba0b-124">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!-- {
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow"
} -->

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "March Proposal.docx",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```
