---
title: Удаление Конверсатионмембер
description: Удаление Конверсатионмембер из канала.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 85fd03831620e338af4dc9ab363fcb9e34fbf971
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002769"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="5632a-103">Удаление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="5632a-103">Delete conversationMember</span></span>

<span data-ttu-id="5632a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5632a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5632a-105">Удаление [конверсатионмембер](../resources/conversationmember.md) из [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="5632a-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="5632a-106">Эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private` .</span><span class="sxs-lookup"><span data-stu-id="5632a-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="5632a-107">Вызовы с любым другим [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="5632a-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="5632a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5632a-108">Permissions</span></span>

<span data-ttu-id="5632a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5632a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5632a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5632a-111">Permission Type</span></span>|<span data-ttu-id="5632a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5632a-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="5632a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5632a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5632a-114">Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5632a-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="5632a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5632a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5632a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5632a-116">Not supported.</span></span>|
|<span data-ttu-id="5632a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5632a-117">Application</span></span>| <span data-ttu-id="5632a-118">Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5632a-118">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5632a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5632a-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5632a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5632a-120">Request headers</span></span>

| <span data-ttu-id="5632a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5632a-121">Header</span></span>       | <span data-ttu-id="5632a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5632a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5632a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5632a-123">Authorization</span></span>  | <span data-ttu-id="5632a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5632a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5632a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5632a-126">Request body</span></span>

<span data-ttu-id="5632a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5632a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5632a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5632a-128">Response</span></span>

<span data-ttu-id="5632a-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5632a-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5632a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5632a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5632a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5632a-131">Request</span></span>

<span data-ttu-id="5632a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5632a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5632a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5632a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="5632a-134">C#</span><span class="sxs-lookup"><span data-stu-id="5632a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5632a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5632a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5632a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5632a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5632a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5632a-137">Response</span></span>

<span data-ttu-id="5632a-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5632a-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


