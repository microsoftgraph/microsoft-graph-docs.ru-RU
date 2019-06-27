---
title: 'group: removeFavorite'
description: Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для Групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: bad40f95743bc7fbfaceebc3aef2b8cbc380d94c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262876"
---
# <a name="group-removefavorite"></a><span data-ttu-id="de8e4-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="de8e4-104">group: removeFavorite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de8e4-p102">Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для Групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="de8e4-p102">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="de8e4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de8e4-107">Permissions</span></span>
<span data-ttu-id="de8e4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de8e4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de8e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de8e4-110">Permission type</span></span>      | <span data-ttu-id="de8e4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de8e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de8e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de8e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="de8e4-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de8e4-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="de8e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de8e4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de8e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de8e4-115">Not supported.</span></span>    |
|<span data-ttu-id="de8e4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de8e4-116">Application</span></span> | <span data-ttu-id="de8e4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de8e4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de8e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de8e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="de8e4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de8e4-119">Request headers</span></span>
| <span data-ttu-id="de8e4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de8e4-120">Header</span></span>       | <span data-ttu-id="de8e4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="de8e4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de8e4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de8e4-122">Authorization</span></span>  | <span data-ttu-id="de8e4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de8e4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="de8e4-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="de8e4-125">Prefer</span></span> | <span data-ttu-id="de8e4-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="de8e4-126">return=minimal.</span></span> <span data-ttu-id="de8e4-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="de8e4-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="de8e4-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="de8e4-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="de8e4-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de8e4-129">Request body</span></span>
<span data-ttu-id="de8e4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de8e4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de8e4-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="de8e4-131">Response</span></span>
<span data-ttu-id="de8e4-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="de8e4-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de8e4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="de8e4-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="de8e4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="de8e4-135">Request</span></span>
<span data-ttu-id="de8e4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de8e4-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="de8e4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="de8e4-137">Response</span></span>
<span data-ttu-id="de8e4-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de8e4-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="de8e4-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="de8e4-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de8e4-140">C#</span><span class="sxs-lookup"><span data-stu-id="de8e4-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_removefavorite-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de8e4-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="de8e4-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_removefavorite-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de8e4-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="de8e4-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_removefavorite-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-removefavorite.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-removefavorite.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-removefavorite.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
