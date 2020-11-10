---
title: Обновление Конверсатионмембер
description: Обновление роли Конверсатионмембер в группе или канале.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 24366fadfb863ba78b8f92ba39c25008c795e23e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956722"
---
# <a name="update-conversationmember"></a><span data-ttu-id="e89db-103">Обновление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="e89db-103">Update conversationMember</span></span>

<span data-ttu-id="e89db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e89db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e89db-105">Обновление роли [конверсатионмембер](../resources/conversationmember.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="e89db-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>
<span data-ttu-id="e89db-106">или [Channel](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="e89db-106">or [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="e89db-107">В каналах эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private` .</span><span class="sxs-lookup"><span data-stu-id="e89db-107">On channels, this operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="e89db-108">Вызовы с любым другим [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="e89db-108">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="e89db-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e89db-109">Permissions</span></span>

<span data-ttu-id="e89db-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e89db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e89db-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e89db-112">Permission Type</span></span>|<span data-ttu-id="e89db-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e89db-113">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="e89db-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e89db-114">Delegated (work or school account)</span></span>| <span data-ttu-id="e89db-115">В teams: Теаммембер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e89db-115">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="e89db-116">В каналах: Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e89db-116">In channels: ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="e89db-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e89db-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e89db-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e89db-118">Not supported</span></span>|
|<span data-ttu-id="e89db-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e89db-119">Application</span></span>| <span data-ttu-id="e89db-120">В teams: Теаммембер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e89db-120">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="e89db-121">В каналах: Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e89db-121">In channels:  ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e89db-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e89db-122">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/members/{id}
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e89db-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e89db-123">Request headers</span></span>

| <span data-ttu-id="e89db-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e89db-124">Header</span></span>       | <span data-ttu-id="e89db-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e89db-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e89db-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e89db-126">Authorization</span></span>  | <span data-ttu-id="e89db-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e89db-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e89db-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e89db-129">Request body</span></span>

<span data-ttu-id="e89db-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e89db-130">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="e89db-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="e89db-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e89db-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e89db-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e89db-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="e89db-133">Property</span></span>   | <span data-ttu-id="e89db-134">Тип</span><span class="sxs-lookup"><span data-stu-id="e89db-134">Type</span></span> |<span data-ttu-id="e89db-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e89db-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e89db-136">roles</span><span class="sxs-lookup"><span data-stu-id="e89db-136">roles</span></span>|<span data-ttu-id="e89db-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e89db-137">string collection</span></span>|<span data-ttu-id="e89db-138">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="e89db-138">The roles for that user.</span></span> <span data-ttu-id="e89db-139">Должен иметь значения "Owner" или "Empty".</span><span class="sxs-lookup"><span data-stu-id="e89db-139">Must be "owner" or empty.</span></span> <span data-ttu-id="e89db-140">Гостевые пользователи всегда должны иметь роль "гость" и не могут измениться.</span><span class="sxs-lookup"><span data-stu-id="e89db-140">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="e89db-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e89db-141">Response</span></span>

<span data-ttu-id="e89db-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e89db-142">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e89db-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e89db-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="e89db-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e89db-144">Request</span></span>

<span data-ttu-id="e89db-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e89db-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e89db-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e89db-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conversation_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="e89db-147">C#</span><span class="sxs-lookup"><span data-stu-id="e89db-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e89db-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e89db-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e89db-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e89db-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e89db-150">Java</span><span class="sxs-lookup"><span data-stu-id="e89db-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e89db-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e89db-151">Response</span></span>

<span data-ttu-id="e89db-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e89db-152">Here is an example of the response.</span></span>

><span data-ttu-id="e89db-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e89db-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


