---
title: Обновление Конверсатионмембер
description: Обновление роли Конверсатионмембер в канале.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d1fad235333e968317d3e4681f56b501016d6352
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634041"
---
# <a name="update-conversationmember"></a><span data-ttu-id="a556a-103">Обновление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="a556a-103">Update conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a556a-104">Обновление роли [конверсатионмембер](../resources/conversationmember.md) в [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="a556a-104">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="a556a-105">Эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private`.</span><span class="sxs-lookup"><span data-stu-id="a556a-105">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="a556a-106">Вызовы с любым другим [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="a556a-106">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="a556a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a556a-107">Permissions</span></span>

<span data-ttu-id="a556a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a556a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a556a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a556a-110">Permission Type</span></span>|<span data-ttu-id="a556a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a556a-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a556a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a556a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a556a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a556a-113">Group.ReadWrite.All</span></span>|
|<span data-ttu-id="a556a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a556a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a556a-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a556a-115">Not supported</span></span>|
|<span data-ttu-id="a556a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a556a-116">Application</span></span>|<span data-ttu-id="a556a-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a556a-117">Group.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a556a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a556a-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a556a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a556a-119">Request headers</span></span>

| <span data-ttu-id="a556a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a556a-120">Header</span></span>       | <span data-ttu-id="a556a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a556a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a556a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a556a-122">Authorization</span></span>  | <span data-ttu-id="a556a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a556a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a556a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a556a-125">Request body</span></span>

<span data-ttu-id="a556a-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a556a-126">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="a556a-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a556a-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a556a-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a556a-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a556a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a556a-129">Property</span></span>   | <span data-ttu-id="a556a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a556a-130">Type</span></span> |<span data-ttu-id="a556a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a556a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a556a-132">roles</span><span class="sxs-lookup"><span data-stu-id="a556a-132">roles</span></span>|<span data-ttu-id="a556a-133">string collection</span><span class="sxs-lookup"><span data-stu-id="a556a-133">string collection</span></span>|<span data-ttu-id="a556a-134">Роли для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a556a-134">The roles for that user.</span></span> <span data-ttu-id="a556a-135">Должен иметь значения "Owner" или "Empty".</span><span class="sxs-lookup"><span data-stu-id="a556a-135">Must be "owner" or empty.</span></span> <span data-ttu-id="a556a-136">Гостевые пользователи всегда должны иметь роль "гость" и не могут измениться.</span><span class="sxs-lookup"><span data-stu-id="a556a-136">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="a556a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a556a-137">Response</span></span>

<span data-ttu-id="a556a-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [конверсатионмембер](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a556a-138">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a556a-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a556a-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="a556a-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a556a-140">Request</span></span>

<span data-ttu-id="a556a-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a556a-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a556a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a556a-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a556a-143">C#</span><span class="sxs-lookup"><span data-stu-id="a556a-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a556a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a556a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a556a-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a556a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a556a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a556a-146">Response</span></span>

<span data-ttu-id="a556a-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a556a-147">Here is an example of the response.</span></span>

><span data-ttu-id="a556a-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a556a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
