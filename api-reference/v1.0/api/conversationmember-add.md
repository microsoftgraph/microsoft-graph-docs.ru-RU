---
title: Добавление conversationMember
description: Добавление conversationMember в канал.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1441ee9698720cc5d5041e7fd3df7c661574077f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053246"
---
# <a name="add-conversationmember"></a><span data-ttu-id="c56ea-103">Добавление conversationMember</span><span class="sxs-lookup"><span data-stu-id="c56ea-103">Add conversationMember</span></span>

<span data-ttu-id="c56ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c56ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c56ea-105">Добавление [conversationMember в](../resources/conversationmember.md) [канал.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="c56ea-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c56ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c56ea-106">Permissions</span></span>

<span data-ttu-id="c56ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c56ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c56ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c56ea-109">Permission Type</span></span>|<span data-ttu-id="c56ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c56ea-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c56ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c56ea-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c56ea-112">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c56ea-112">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="c56ea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c56ea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c56ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c56ea-114">Not supported.</span></span>|
|<span data-ttu-id="c56ea-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c56ea-115">Application</span></span>| <span data-ttu-id="c56ea-116">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c56ea-116">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c56ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c56ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members
```

## <a name="request-headers"></a><span data-ttu-id="c56ea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c56ea-118">Request headers</span></span>

| <span data-ttu-id="c56ea-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c56ea-119">Header</span></span>       | <span data-ttu-id="c56ea-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c56ea-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c56ea-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c56ea-121">Authorization</span></span>  | <span data-ttu-id="c56ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c56ea-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c56ea-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c56ea-124">Request body</span></span>

<span data-ttu-id="c56ea-125">Включите в запрос указанные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="c56ea-125">Include the following properties in the request body.</span></span>

| <span data-ttu-id="c56ea-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c56ea-126">Property</span></span>   | <span data-ttu-id="c56ea-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c56ea-127">Type</span></span> |<span data-ttu-id="c56ea-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c56ea-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c56ea-129">roles</span><span class="sxs-lookup"><span data-stu-id="c56ea-129">roles</span></span>|<span data-ttu-id="c56ea-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c56ea-130">string collection</span></span>|<span data-ttu-id="c56ea-131">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c56ea-131">The roles for that user.</span></span>|
|<span data-ttu-id="c56ea-132">user</span><span class="sxs-lookup"><span data-stu-id="c56ea-132">user</span></span>|[<span data-ttu-id="c56ea-133">user</span><span class="sxs-lookup"><span data-stu-id="c56ea-133">user</span></span>](../resources/user.md)|<span data-ttu-id="c56ea-134">Пользователь, который должен добавить в канал.</span><span class="sxs-lookup"><span data-stu-id="c56ea-134">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="c56ea-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c56ea-135">Response</span></span>

<span data-ttu-id="c56ea-136">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c56ea-136">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c56ea-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c56ea-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c56ea-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c56ea-138">Request</span></span>

<span data-ttu-id="c56ea-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c56ea-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c56ea-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c56ea-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member"
} -->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/members/
content-type: application/json
content-length: 26

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "roles": [],
  "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="c56ea-141">C#</span><span class="sxs-lookup"><span data-stu-id="c56ea-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c56ea-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c56ea-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c56ea-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c56ea-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c56ea-144">Java</span><span class="sxs-lookup"><span data-stu-id="c56ea-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c56ea-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c56ea-145">Response</span></span>

<span data-ttu-id="c56ea-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c56ea-146">Here is an example of the response.</span></span>

><span data-ttu-id="c56ea-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c56ea-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/V1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
