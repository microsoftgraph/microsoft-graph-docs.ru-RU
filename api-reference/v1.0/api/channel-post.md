---
title: Создание канала
description: Создание канала в Microsoft Team, как указано в тексте запроса.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: bdf98d5bdfe49ca45e715d4eb6d63f0a514548b6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273670"
---
# <a name="create-channel"></a><span data-ttu-id="5cada-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="5cada-103">Create Channel</span></span>



<span data-ttu-id="5cada-104">Создание [канала](../resources/channel.md) в Microsoft Team, как указано в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="5cada-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="5cada-105">**Примечание**. Существует известная проблема с разрешениями для приложений и этим API.</span><span class="sxs-lookup"><span data-stu-id="5cada-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="5cada-106">Дополнительные сведения см. в [списке известных проблем](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="5cada-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="5cada-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cada-107">Permissions</span></span>
<span data-ttu-id="5cada-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cada-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5cada-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cada-110">Permission type</span></span>      | <span data-ttu-id="5cada-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cada-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cada-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cada-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5cada-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cada-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5cada-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cada-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cada-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cada-115">Not supported.</span></span>    |
|<span data-ttu-id="5cada-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cada-116">Application</span></span> | <span data-ttu-id="5cada-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cada-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="5cada-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="5cada-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5cada-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="5cada-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5cada-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cada-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="5cada-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cada-121">Request headers</span></span>
| <span data-ttu-id="5cada-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cada-122">Header</span></span>       | <span data-ttu-id="5cada-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5cada-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5cada-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cada-124">Authorization</span></span>  | <span data-ttu-id="5cada-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cada-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5cada-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5cada-127">Content-Type</span></span>  | <span data-ttu-id="5cada-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5cada-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cada-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cada-129">Request body</span></span>
<span data-ttu-id="5cada-130">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cada-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5cada-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cada-131">Response</span></span>

<span data-ttu-id="5cada-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cada-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cada-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5cada-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cada-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cada-134">Request</span></span>
<span data-ttu-id="5cada-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cada-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="5cada-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cada-136">Response</span></span>
<span data-ttu-id="5cada-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5cada-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5cada-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5cada-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5cada-141">C#</span><span class="sxs-lookup"><span data-stu-id="5cada-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_channel_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5cada-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cada-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_channel_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5cada-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5cada-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_channel_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/channel-post.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/channel-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/channel-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
