---
title: Добавление Конверсатионмембер
description: Добавление Конверсатионмембер к каналу.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 40ed8afa7700bc2fa1639986c336d15130b03a57
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050759"
---
# <a name="add-conversationmember"></a><span data-ttu-id="2a65f-103">Добавление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="2a65f-103">Add conversationMember</span></span>

<span data-ttu-id="2a65f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a65f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a65f-105">Добавление [конверсатионмембер](../resources/conversationmember.md) к [каналу](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="2a65f-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span>

> [!NOTE]
><span data-ttu-id="2a65f-106">Эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private` .</span><span class="sxs-lookup"><span data-stu-id="2a65f-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="2a65f-107">Вызовы с любыми другими [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать ответ о неправильном запросе 400.</span><span class="sxs-lookup"><span data-stu-id="2a65f-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a 400 Bad Request response.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a65f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a65f-108">Permissions</span></span>

<span data-ttu-id="2a65f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2a65f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2a65f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a65f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a65f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a65f-111">Permission Type</span></span>|<span data-ttu-id="2a65f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a65f-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="2a65f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a65f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2a65f-114">Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2a65f-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="2a65f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a65f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a65f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a65f-116">Not supported.</span></span>|
|<span data-ttu-id="2a65f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2a65f-117">Application</span></span>| <span data-ttu-id="2a65f-118">Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2a65f-118">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a65f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a65f-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members
```

## <a name="request-headers"></a><span data-ttu-id="2a65f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a65f-120">Request headers</span></span>

| <span data-ttu-id="2a65f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a65f-121">Header</span></span>       | <span data-ttu-id="2a65f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2a65f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a65f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a65f-123">Authorization</span></span>  | <span data-ttu-id="2a65f-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="2a65f-124">Bearer {token}.</span></span> <span data-ttu-id="2a65f-125">Required.</span><span class="sxs-lookup"><span data-stu-id="2a65f-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a65f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a65f-126">Request body</span></span>

<span data-ttu-id="2a65f-127">Включите в запрос указанные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="2a65f-127">Include the following properties in the request body.</span></span>

| <span data-ttu-id="2a65f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a65f-128">Property</span></span>   | <span data-ttu-id="2a65f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2a65f-129">Type</span></span> |<span data-ttu-id="2a65f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2a65f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a65f-131">roles</span><span class="sxs-lookup"><span data-stu-id="2a65f-131">roles</span></span>|<span data-ttu-id="2a65f-132">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2a65f-132">string collection</span></span>|<span data-ttu-id="2a65f-133">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a65f-133">The roles for that user.</span></span>|
|<span data-ttu-id="2a65f-134">пользователь;</span><span class="sxs-lookup"><span data-stu-id="2a65f-134">user</span></span>|[<span data-ttu-id="2a65f-135">user</span><span class="sxs-lookup"><span data-stu-id="2a65f-135">user</span></span>](../resources/user.md)|<span data-ttu-id="2a65f-136">Пользователь, добавляемый в канал.</span><span class="sxs-lookup"><span data-stu-id="2a65f-136">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="2a65f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a65f-137">Response</span></span>

<span data-ttu-id="2a65f-138">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2a65f-138">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a65f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="2a65f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a65f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a65f-140">Request</span></span>

<span data-ttu-id="2a65f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a65f-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a65f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a65f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member"
} -->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/
content-type: application/json
content-length: 26

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "roles": [],
  "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="2a65f-143">C#</span><span class="sxs-lookup"><span data-stu-id="2a65f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a65f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a65f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a65f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a65f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a65f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a65f-146">Response</span></span>

<span data-ttu-id="2a65f-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2a65f-147">Here is an example of the response.</span></span>

><span data-ttu-id="2a65f-148">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="2a65f-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2a65f-149">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2a65f-149">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
