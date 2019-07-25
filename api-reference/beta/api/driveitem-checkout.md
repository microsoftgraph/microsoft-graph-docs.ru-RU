---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Извлечение файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e92af4dea2e5b0678e72bc3311042acba9266a5b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861410"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="b7e4c-102">Получение ресурса DriveItem для изменения</span><span class="sxs-lookup"><span data-stu-id="b7e4c-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7e4c-103">Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет [записан после изменения](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="b7e4c-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7e4c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7e4c-104">Permissions</span></span>

<span data-ttu-id="b7e4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7e4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7e4c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7e4c-107">Permission type</span></span>      | <span data-ttu-id="b7e4c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7e4c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7e4c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7e4c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b7e4c-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e4c-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7e4c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7e4c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7e4c-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e4c-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7e4c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7e4c-113">Application</span></span> | <span data-ttu-id="b7e4c-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e4c-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7e4c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7e4c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="b7e4c-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7e4c-116">Request body</span></span>

<span data-ttu-id="b7e4c-117">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="b7e4c-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="b7e4c-118">Пример</span><span class="sxs-lookup"><span data-stu-id="b7e4c-118">Example</span></span>

<span data-ttu-id="b7e4c-119">В этом примере показано, как записать после изменения файл, указанный по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="b7e4c-119">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b7e4c-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7e4c-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7e4c-121">C#</span><span class="sxs-lookup"><span data-stu-id="b7e4c-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7e4c-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="b7e4c-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7e4c-123">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b7e4c-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b7e4c-124">Java</span><span class="sxs-lookup"><span data-stu-id="b7e4c-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkout-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="b7e4c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7e4c-125">Response</span></span>

<span data-ttu-id="b7e4c-126">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="b7e4c-126">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="b7e4c-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="b7e4c-127">Remarks</span></span>


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
