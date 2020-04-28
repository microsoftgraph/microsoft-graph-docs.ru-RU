---
title: Добавление Конверсатионмембер
description: Добавление Конверсатионмембер к каналу.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5e48c3751daf58ac9fdbb3e7c090ea9147364d5a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436582"
---
# <a name="add-conversationmember"></a><span data-ttu-id="ac8ba-103">Добавление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="ac8ba-103">Add conversationMember</span></span>

<span data-ttu-id="ac8ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac8ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac8ba-105">Добавление [конверсатионмембер](../resources/conversationmember.md) к [каналу](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ac8ba-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span>

> [!NOTE]
><span data-ttu-id="ac8ba-106">Эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private`.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="ac8ba-107">Вызовы с любыми другими [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать ответ о неправильном запросе 400.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a 400 Bad Request response.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac8ba-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac8ba-108">Permissions</span></span>

<span data-ttu-id="ac8ba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac8ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac8ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac8ba-111">Permission Type</span></span>|<span data-ttu-id="ac8ba-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac8ba-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ac8ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac8ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac8ba-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac8ba-114">Group.ReadWrite.All</span></span>|
|<span data-ttu-id="ac8ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac8ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac8ba-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ac8ba-116">Not supported</span></span>|
|<span data-ttu-id="ac8ba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac8ba-117">Application</span></span>|<span data-ttu-id="ac8ba-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac8ba-118">Group.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac8ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac8ba-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members
```

## <a name="request-headers"></a><span data-ttu-id="ac8ba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac8ba-120">Request headers</span></span>

| <span data-ttu-id="ac8ba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac8ba-121">Header</span></span>       | <span data-ttu-id="ac8ba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ac8ba-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac8ba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac8ba-123">Authorization</span></span>  | <span data-ttu-id="ac8ba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac8ba-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac8ba-126">Request body</span></span>

<span data-ttu-id="ac8ba-127">Включите в запрос указанные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-127">Include the following properties in the request body.</span></span>

| <span data-ttu-id="ac8ba-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac8ba-128">Property</span></span>   | <span data-ttu-id="ac8ba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ac8ba-129">Type</span></span> |<span data-ttu-id="ac8ba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ac8ba-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac8ba-131">roles</span><span class="sxs-lookup"><span data-stu-id="ac8ba-131">roles</span></span>|<span data-ttu-id="ac8ba-132">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ac8ba-132">string collection</span></span>|<span data-ttu-id="ac8ba-133">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-133">The roles for that user.</span></span>|
|<span data-ttu-id="ac8ba-134">user</span><span class="sxs-lookup"><span data-stu-id="ac8ba-134">user</span></span>|[<span data-ttu-id="ac8ba-135">user</span><span class="sxs-lookup"><span data-stu-id="ac8ba-135">user</span></span>](../resources/user.md)|<span data-ttu-id="ac8ba-136">Пользователь, добавляемый в канал.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-136">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="ac8ba-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac8ba-137">Response</span></span>

<span data-ttu-id="ac8ba-138">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-138">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac8ba-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ac8ba-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac8ba-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac8ba-140">Request</span></span>

<span data-ttu-id="ac8ba-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac8ba-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac8ba-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ac8ba-143">C#</span><span class="sxs-lookup"><span data-stu-id="ac8ba-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac8ba-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac8ba-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac8ba-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac8ba-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac8ba-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac8ba-146">Response</span></span>

<span data-ttu-id="ac8ba-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-147">Here is an example of the response.</span></span>

><span data-ttu-id="ac8ba-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac8ba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
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
