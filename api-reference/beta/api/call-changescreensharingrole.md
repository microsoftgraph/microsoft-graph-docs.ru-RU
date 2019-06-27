---
title: 'Call: Чанжескриншарингроле'
description: Начало и прекращение демонстрации экрана в звонке. Этот API используется, чтобы разрешить приложениям совместно использовать содержимое экрана с участниками звонка или собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 87a2c56810d80af8f38e0a3b7ae84b5c6f787e22
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262326"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="96d34-104">Call: Чанжескриншарингроле</span><span class="sxs-lookup"><span data-stu-id="96d34-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96d34-105">Начало и прекращение демонстрации экрана в звонке.</span><span class="sxs-lookup"><span data-stu-id="96d34-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="96d34-106">Этот API используется, чтобы разрешить приложениям совместно использовать содержимое экрана с участниками звонка или собрания.</span><span class="sxs-lookup"><span data-stu-id="96d34-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="96d34-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96d34-107">Permissions</span></span>
<span data-ttu-id="96d34-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96d34-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96d34-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96d34-110">Permission type</span></span>                        | <span data-ttu-id="96d34-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96d34-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="96d34-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96d34-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="96d34-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96d34-113">Not Supported</span></span>                               |
| <span data-ttu-id="96d34-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96d34-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96d34-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96d34-115">Not Supported</span></span>                               |
| <span data-ttu-id="96d34-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96d34-116">Application</span></span>                            | <span data-ttu-id="96d34-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="96d34-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="96d34-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96d34-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="96d34-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96d34-119">Request headers</span></span>
| <span data-ttu-id="96d34-120">Имя</span><span class="sxs-lookup"><span data-stu-id="96d34-120">Name</span></span>          | <span data-ttu-id="96d34-121">Описание</span><span class="sxs-lookup"><span data-stu-id="96d34-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="96d34-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96d34-122">Authorization</span></span> | <span data-ttu-id="96d34-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96d34-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96d34-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96d34-125">Request body</span></span>
<span data-ttu-id="96d34-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="96d34-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96d34-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="96d34-127">Parameter</span></span>      | <span data-ttu-id="96d34-128">Тип</span><span class="sxs-lookup"><span data-stu-id="96d34-128">Type</span></span>    |<span data-ttu-id="96d34-129">Описание</span><span class="sxs-lookup"><span data-stu-id="96d34-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96d34-130">role</span><span class="sxs-lookup"><span data-stu-id="96d34-130">role</span></span>|<span data-ttu-id="96d34-131">String</span><span class="sxs-lookup"><span data-stu-id="96d34-131">String</span></span>|<span data-ttu-id="96d34-132">Возможные значения: "средство просмотра", "общий доступ"</span><span class="sxs-lookup"><span data-stu-id="96d34-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="96d34-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="96d34-133">Response</span></span>
<span data-ttu-id="96d34-134">Возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="96d34-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="96d34-135">Пример</span><span class="sxs-lookup"><span data-stu-id="96d34-135">Example</span></span>
<span data-ttu-id="96d34-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="96d34-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="96d34-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="96d34-137">Request</span></span>
<span data-ttu-id="96d34-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96d34-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="96d34-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="96d34-139">Response</span></span>
<span data-ttu-id="96d34-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96d34-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="96d34-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="96d34-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="96d34-142">C#</span><span class="sxs-lookup"><span data-stu-id="96d34-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-changeScreenSharingRole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96d34-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="96d34-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-changeScreenSharingRole-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="96d34-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="96d34-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/call-changeScreenSharingRole-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
