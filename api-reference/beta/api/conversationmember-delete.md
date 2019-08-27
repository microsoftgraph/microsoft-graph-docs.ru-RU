---
title: Удаление Конверсатионмембер
description: Удаление Конверсатионмембер из канала.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 739705d2c57210d15813ad8cbed4627afef29d07
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634052"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="93a1e-103">Удаление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="93a1e-103">Delete conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93a1e-104">Удаление [конверсатионмембер](../resources/conversationmember.md) из [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="93a1e-104">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="93a1e-105">Эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private`.</span><span class="sxs-lookup"><span data-stu-id="93a1e-105">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="93a1e-106">Вызовы с любым другим [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="93a1e-106">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="93a1e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93a1e-107">Permissions</span></span>

<span data-ttu-id="93a1e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93a1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93a1e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93a1e-110">Permission Type</span></span>|<span data-ttu-id="93a1e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93a1e-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="93a1e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93a1e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93a1e-113">Для ресурса **User** или **Chat** :</span><span class="sxs-lookup"><span data-stu-id="93a1e-113">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="93a1e-114">Чат. Read, Chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93a1e-114">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="93a1e-115">Для ресурса **Channel** :</span><span class="sxs-lookup"><span data-stu-id="93a1e-115">For **channel** resource:</span></span><br/><span data-ttu-id="93a1e-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93a1e-116">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="93a1e-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93a1e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93a1e-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="93a1e-118">Not supported</span></span>|
|<span data-ttu-id="93a1e-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93a1e-119">Application</span></span>| <span data-ttu-id="93a1e-120">Для ресурса **User** или **Chat** :</span><span class="sxs-lookup"><span data-stu-id="93a1e-120">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="93a1e-121">Чат. Read. ALL, Chat. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="93a1e-121">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="93a1e-122">Для ресурса **Channel** :</span><span class="sxs-lookup"><span data-stu-id="93a1e-122">For **channel** resource:</span></span><br/><span data-ttu-id="93a1e-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93a1e-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93a1e-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93a1e-124">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="93a1e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93a1e-125">Request headers</span></span>

| <span data-ttu-id="93a1e-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93a1e-126">Header</span></span>       | <span data-ttu-id="93a1e-127">Значение</span><span class="sxs-lookup"><span data-stu-id="93a1e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="93a1e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93a1e-128">Authorization</span></span>  | <span data-ttu-id="93a1e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93a1e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93a1e-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93a1e-131">Request body</span></span>

<span data-ttu-id="93a1e-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93a1e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93a1e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="93a1e-133">Response</span></span>

<span data-ttu-id="93a1e-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="93a1e-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="93a1e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="93a1e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="93a1e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="93a1e-136">Request</span></span>

<span data-ttu-id="93a1e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93a1e-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="93a1e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="93a1e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93a1e-139">C#</span><span class="sxs-lookup"><span data-stu-id="93a1e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93a1e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93a1e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93a1e-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="93a1e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93a1e-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="93a1e-142">Response</span></span>

<span data-ttu-id="93a1e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93a1e-143">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
