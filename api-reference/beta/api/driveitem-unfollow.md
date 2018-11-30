---
author: chackman
ms.author: chackman
title: Отменить подписку на диске элемента
ms.openlocfilehash: 871ea9782e62e66adeed743819a265b452e06de3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075017"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="0e52f-102">Отменить подписку на диске элемента</span><span class="sxs-lookup"><span data-stu-id="0e52f-102">Unfollow drive item</span></span>

> <span data-ttu-id="0e52f-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e52f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e52f-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e52f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e52f-105">Отменить подписку на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0e52f-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="0e52f-106">**Примечание:** Для выполнения элемента, видите [Выполните элемента](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="0e52f-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e52f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e52f-107">Permissions</span></span>

<span data-ttu-id="0e52f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e52f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e52f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e52f-110">Permission type</span></span>      | <span data-ttu-id="0e52f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e52f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e52f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e52f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0e52f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e52f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e52f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e52f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e52f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e52f-115">Not supported.</span></span>    |
|<span data-ttu-id="0e52f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e52f-116">Application</span></span> | <span data-ttu-id="0e52f-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e52f-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e52f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e52f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="0e52f-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e52f-119">Request body</span></span>

<span data-ttu-id="0e52f-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="0e52f-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="0e52f-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e52f-121">Response</span></span>

<span data-ttu-id="0e52f-122">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0e52f-122">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="0e52f-123">Пример</span><span class="sxs-lookup"><span data-stu-id="0e52f-123">Example</span></span>

<span data-ttu-id="0e52f-124">В этом примере unfollows элемент, определенный с `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="0e52f-124">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```


<!-- {
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow"
} -->
