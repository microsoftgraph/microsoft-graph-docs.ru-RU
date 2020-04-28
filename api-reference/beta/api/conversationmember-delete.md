---
title: Удаление Конверсатионмембер
description: Удаление Конверсатионмембер из канала.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0a6ac8b72f5dea24c0f60062b91dac7648b91e85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436568"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="5db2a-103">Удаление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="5db2a-103">Delete conversationMember</span></span>

<span data-ttu-id="5db2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5db2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5db2a-105">Удаление [конверсатионмембер](../resources/conversationmember.md) из [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="5db2a-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="5db2a-106">Эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private`.</span><span class="sxs-lookup"><span data-stu-id="5db2a-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="5db2a-107">Вызовы с любым другим [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="5db2a-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="5db2a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5db2a-108">Permissions</span></span>

<span data-ttu-id="5db2a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5db2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5db2a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5db2a-111">Permission Type</span></span>|<span data-ttu-id="5db2a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5db2a-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="5db2a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5db2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5db2a-114">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="5db2a-114">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="5db2a-115">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5db2a-115">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="5db2a-116">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="5db2a-116">For **channel** resource:</span></span><br/><span data-ttu-id="5db2a-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db2a-117">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="5db2a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5db2a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5db2a-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5db2a-119">Not supported</span></span>|
|<span data-ttu-id="5db2a-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="5db2a-120">Application</span></span>| <span data-ttu-id="5db2a-121">Для ресурса **user** или **chat**:</span><span class="sxs-lookup"><span data-stu-id="5db2a-121">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="5db2a-122">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db2a-122">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="5db2a-123">Для ресурса **channel**:</span><span class="sxs-lookup"><span data-stu-id="5db2a-123">For **channel** resource:</span></span><br/><span data-ttu-id="5db2a-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db2a-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5db2a-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5db2a-125">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5db2a-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5db2a-126">Request headers</span></span>

| <span data-ttu-id="5db2a-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5db2a-127">Header</span></span>       | <span data-ttu-id="5db2a-128">Значение</span><span class="sxs-lookup"><span data-stu-id="5db2a-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5db2a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5db2a-129">Authorization</span></span>  | <span data-ttu-id="5db2a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5db2a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5db2a-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5db2a-132">Request body</span></span>

<span data-ttu-id="5db2a-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5db2a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5db2a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5db2a-134">Response</span></span>

<span data-ttu-id="5db2a-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5db2a-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5db2a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5db2a-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5db2a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5db2a-137">Request</span></span>

<span data-ttu-id="5db2a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5db2a-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5db2a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5db2a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="5db2a-140">C#</span><span class="sxs-lookup"><span data-stu-id="5db2a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5db2a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5db2a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5db2a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5db2a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5db2a-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="5db2a-143">Response</span></span>

<span data-ttu-id="5db2a-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5db2a-144">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
