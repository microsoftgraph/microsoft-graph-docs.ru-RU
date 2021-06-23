---
title: Удаление участника из канала
description: Удалите участника из канала.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ae46702936fb82ac00c0744927c1d5b0b2ccc6dd
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060029"
---
# <a name="remove-member-from-channel"></a><span data-ttu-id="9f331-103">Удаление участника из канала</span><span class="sxs-lookup"><span data-stu-id="9f331-103">Remove member from channel</span></span>

<span data-ttu-id="9f331-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f331-104">Namespace: microsoft.graph</span></span>
 
<span data-ttu-id="9f331-105">Удаление [conversationMember из](../resources/conversationmember.md) [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="9f331-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span> <span data-ttu-id="9f331-106">Эта операция разрешена только для каналов со значением **membershipType** `private` .</span><span class="sxs-lookup"><span data-stu-id="9f331-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>


## <a name="permissions"></a><span data-ttu-id="9f331-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f331-107">Permissions</span></span>

<span data-ttu-id="9f331-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f331-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f331-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f331-110">Permission Type</span></span>|<span data-ttu-id="9f331-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f331-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9f331-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f331-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9f331-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f331-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="9f331-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f331-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f331-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f331-115">Not supported.</span></span>|
|<span data-ttu-id="9f331-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f331-116">Application</span></span>| <span data-ttu-id="9f331-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f331-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f331-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f331-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->

```http
DELETE /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="9f331-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f331-119">Request headers</span></span>

| <span data-ttu-id="9f331-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f331-120">Header</span></span>       | <span data-ttu-id="9f331-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f331-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f331-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f331-122">Authorization</span></span>  | <span data-ttu-id="9f331-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f331-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f331-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f331-125">Request body</span></span>

<span data-ttu-id="9f331-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f331-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f331-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f331-127">Response</span></span>

<span data-ttu-id="9f331-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9f331-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9f331-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9f331-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f331-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f331-130">Request</span></span>

<span data-ttu-id="9f331-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f331-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9f331-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f331-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel-member"
} -->
```http
DELETE https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="9f331-133">C#</span><span class="sxs-lookup"><span data-stu-id="9f331-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f331-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f331-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f331-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f331-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f331-136">Java</span><span class="sxs-lookup"><span data-stu-id="9f331-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-channel-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9f331-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f331-137">Response</span></span>

<span data-ttu-id="9f331-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f331-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="9f331-139">См. также</span><span class="sxs-lookup"><span data-stu-id="9f331-139">See also</span></span>

- [<span data-ttu-id="9f331-140">Удаление участника из чата</span><span class="sxs-lookup"><span data-stu-id="9f331-140">Remove member from team</span></span>](team-delete-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete_channel_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
