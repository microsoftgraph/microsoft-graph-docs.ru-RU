---
title: Обновление Конверсатионмембер
description: Обновление роли Конверсатионмембер в канале.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b380d6c274c2d0ca2771cd44a7015f84f7d9a0e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436421"
---
# <a name="update-conversationmember"></a><span data-ttu-id="9579e-103">Обновление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="9579e-103">Update conversationMember</span></span>

<span data-ttu-id="9579e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9579e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9579e-105">Обновление роли [конверсатионмембер](../resources/conversationmember.md) в [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="9579e-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="9579e-106">Эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private`.</span><span class="sxs-lookup"><span data-stu-id="9579e-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="9579e-107">Вызовы с любым другим [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="9579e-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="9579e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9579e-108">Permissions</span></span>

<span data-ttu-id="9579e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9579e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9579e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9579e-111">Permission Type</span></span>|<span data-ttu-id="9579e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9579e-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9579e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9579e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9579e-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9579e-114">Group.ReadWrite.All</span></span>|
|<span data-ttu-id="9579e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9579e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9579e-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9579e-116">Not supported</span></span>|
|<span data-ttu-id="9579e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9579e-117">Application</span></span>|<span data-ttu-id="9579e-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9579e-118">Group.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9579e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9579e-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9579e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9579e-120">Request headers</span></span>

| <span data-ttu-id="9579e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9579e-121">Header</span></span>       | <span data-ttu-id="9579e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9579e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9579e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9579e-123">Authorization</span></span>  | <span data-ttu-id="9579e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9579e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9579e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9579e-126">Request body</span></span>

<span data-ttu-id="9579e-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9579e-127">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="9579e-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="9579e-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9579e-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9579e-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9579e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9579e-130">Property</span></span>   | <span data-ttu-id="9579e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9579e-131">Type</span></span> |<span data-ttu-id="9579e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9579e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9579e-133">roles</span><span class="sxs-lookup"><span data-stu-id="9579e-133">roles</span></span>|<span data-ttu-id="9579e-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9579e-134">string collection</span></span>|<span data-ttu-id="9579e-135">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9579e-135">The roles for that user.</span></span> <span data-ttu-id="9579e-136">Должен иметь значения "Owner" или "Empty".</span><span class="sxs-lookup"><span data-stu-id="9579e-136">Must be "owner" or empty.</span></span> <span data-ttu-id="9579e-137">Гостевые пользователи всегда должны иметь роль "гость" и не могут измениться.</span><span class="sxs-lookup"><span data-stu-id="9579e-137">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="9579e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9579e-138">Response</span></span>

<span data-ttu-id="9579e-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9579e-139">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9579e-140">Пример</span><span class="sxs-lookup"><span data-stu-id="9579e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9579e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="9579e-141">Request</span></span>

<span data-ttu-id="9579e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9579e-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9579e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9579e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conversation_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
content-type: application/json
content-length: 26

{
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="9579e-144">C#</span><span class="sxs-lookup"><span data-stu-id="9579e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9579e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9579e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9579e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9579e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9579e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9579e-147">Response</span></span>

<span data-ttu-id="9579e-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9579e-148">Here is an example of the response.</span></span>

><span data-ttu-id="9579e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9579e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 475

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
