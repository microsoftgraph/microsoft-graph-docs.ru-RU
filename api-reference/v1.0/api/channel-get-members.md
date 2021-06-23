---
title: Получение участника канала
description: Получение участника канала.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6aeb2f24822995e9e2a9d9e153182842b8d99ff
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060560"
---
# <a name="get-member-of-channel"></a><span data-ttu-id="71aff-103">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="71aff-103">Get member of channel</span></span>

<span data-ttu-id="71aff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71aff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71aff-105">Получение [conversationMember](../resources/conversationmember.md) из [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="71aff-105">Get a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71aff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71aff-106">Permissions</span></span>

<span data-ttu-id="71aff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71aff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71aff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71aff-109">Permission Type</span></span>|<span data-ttu-id="71aff-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71aff-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="71aff-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71aff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71aff-112">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71aff-112">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="71aff-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71aff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71aff-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71aff-114">Not supported.</span></span>|
|<span data-ttu-id="71aff-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="71aff-115">Application</span></span>|<span data-ttu-id="71aff-116">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71aff-116">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="71aff-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71aff-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
GET /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71aff-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71aff-118">Optional query parameters</span></span>

<span data-ttu-id="71aff-119">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="71aff-119">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71aff-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71aff-120">Request headers</span></span>

| <span data-ttu-id="71aff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71aff-121">Header</span></span>       | <span data-ttu-id="71aff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71aff-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71aff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71aff-123">Authorization</span></span>  | <span data-ttu-id="71aff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71aff-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71aff-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71aff-126">Request body</span></span>

<span data-ttu-id="71aff-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71aff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71aff-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="71aff-128">Response</span></span>

<span data-ttu-id="71aff-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71aff-129">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71aff-130">Пример</span><span class="sxs-lookup"><span data-stu-id="71aff-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="71aff-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="71aff-131">Request</span></span>

<span data-ttu-id="71aff-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71aff-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71aff-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="71aff-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel-get_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="71aff-134">C#</span><span class="sxs-lookup"><span data-stu-id="71aff-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-get-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71aff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71aff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-get-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71aff-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71aff-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-get-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71aff-137">Java</span><span class="sxs-lookup"><span data-stu-id="71aff-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-get-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71aff-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="71aff-138">Response</span></span>

<span data-ttu-id="71aff-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71aff-139">Here is an example of the response.</span></span>

><span data-ttu-id="71aff-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71aff-140">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
   "@odata.type":"#microsoft.graph.aadUserConversationMember",
   "id":"ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
   "roles":[
      "owner"
   ],
   "displayName":"John Doe",
   "userId":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
   "email":null
}
```

## <a name="see-also"></a><span data-ttu-id="71aff-141">См. также</span><span class="sxs-lookup"><span data-stu-id="71aff-141">See also</span></span>

- [<span data-ttu-id="71aff-142">Получение участника команды</span><span class="sxs-lookup"><span data-stu-id="71aff-142">Get member of team</span></span>](team-get-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "get_channel_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
