---
title: 'group: subscribeByMail'
description: Вызов этого метода позволит текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлах в этой группе. Поддерживается только для групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 6795257a1a86049457ddb475356280980e9a203e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277632"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="4cfe7-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="4cfe7-104">group: subscribeByMail</span></span>
<span data-ttu-id="4cfe7-p102">Вызов этого метода позволит текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлах в этой группе. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-p102">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cfe7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cfe7-107">Permissions</span></span>
<span data-ttu-id="4cfe7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cfe7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cfe7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cfe7-110">Permission type</span></span>      | <span data-ttu-id="4cfe7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cfe7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cfe7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cfe7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4cfe7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfe7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4cfe7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cfe7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cfe7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-115">Not supported.</span></span>    |
|<span data-ttu-id="4cfe7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cfe7-116">Application</span></span> | <span data-ttu-id="4cfe7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cfe7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cfe7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="4cfe7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cfe7-119">Request headers</span></span>
| <span data-ttu-id="4cfe7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cfe7-120">Header</span></span>       | <span data-ttu-id="4cfe7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4cfe7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4cfe7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cfe7-122">Authorization</span></span>  | <span data-ttu-id="4cfe7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4cfe7-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="4cfe7-125">Prefer</span></span> | <span data-ttu-id="4cfe7-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-126">return=minimal.</span></span> <span data-ttu-id="4cfe7-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="4cfe7-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="4cfe7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cfe7-129">Request body</span></span>
<span data-ttu-id="4cfe7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cfe7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cfe7-131">Response</span></span>
<span data-ttu-id="4cfe7-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cfe7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="4cfe7-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4cfe7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cfe7-135">Request</span></span>
<span data-ttu-id="4cfe7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="4cfe7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cfe7-137">Response</span></span>
<span data-ttu-id="4cfe7-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4cfe7-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4cfe7-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4cfe7-140">C#</span><span class="sxs-lookup"><span data-stu-id="4cfe7-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_subscribebymail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4cfe7-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="4cfe7-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_subscribebymail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4cfe7-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4cfe7-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_subscribebymail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-subscribebymail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-subscribebymail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-subscribebymail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
