---
title: Обновление chatMessage
description: Обновление свойства policyViolation объекта chatMessage.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d5d4b36f2d0ca0ef3d62c3991feae64a8e57a700
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115236"
---
# <a name="update-chatmessage"></a><span data-ttu-id="5248d-103">Обновление chatMessage</span><span class="sxs-lookup"><span data-stu-id="5248d-103">Update chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="5248d-104">Обновление объекта [chatMessage.](../resources/chatMessage.md)</span><span class="sxs-lookup"><span data-stu-id="5248d-104">Update a [chatMessage](../resources/chatMessage.md) object.</span></span> <span data-ttu-id="5248d-105">Обновлять можно только свойство **policyViolation** **объекта chatMessage.**</span><span class="sxs-lookup"><span data-stu-id="5248d-105">Only the **policyViolation** property of a **chatMessage** can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="5248d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5248d-106">Permissions</span></span>

<span data-ttu-id="5248d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5248d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5248d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5248d-109">Permission type</span></span>      | <span data-ttu-id="5248d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5248d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5248d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5248d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5248d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5248d-112">Not supported.</span></span> |
|<span data-ttu-id="5248d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5248d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5248d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5248d-114">Not supported.</span></span>    |
|<span data-ttu-id="5248d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5248d-115">Application</span></span> | <span data-ttu-id="5248d-116">Chat.UpdatePolicyViolation.All для сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="5248d-116">Chat.UpdatePolicyViolation.All for a chat message.</span></span></br><span data-ttu-id="5248d-117">ChannelMessage.UpdatePolicyViolation.All для сообщения канала.</span><span class="sxs-lookup"><span data-stu-id="5248d-117">ChannelMessage.UpdatePolicyViolation.All for a channel message.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5248d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5248d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/(team-id)/channels/{channel-id}/messages/{message-id}
PATCH /chats/{chatThread-id}/messages/{message-id}
```

## <a name="request-headers"></a><span data-ttu-id="5248d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5248d-119">Request headers</span></span>

| <span data-ttu-id="5248d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5248d-120">Name</span></span>       | <span data-ttu-id="5248d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5248d-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5248d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5248d-122">Authorization</span></span>  | <span data-ttu-id="5248d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5248d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5248d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5248d-125">Content-Type</span></span> | <span data-ttu-id="5248d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5248d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5248d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5248d-128">Request body</span></span>

<span data-ttu-id="5248d-129">В теле запроса укажите представление объекта [chatMessage](../resources/chatMessage.md) в JSON, указав только **свойство policyViolation.**</span><span class="sxs-lookup"><span data-stu-id="5248d-129">In the request body, supply a JSON representation of a [chatMessage](../resources/chatMessage.md) object, specifying only the **policyViolation** property.</span></span>

## <a name="response"></a><span data-ttu-id="5248d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5248d-130">Response</span></span>

<span data-ttu-id="5248d-131">В случае успеха этот метод возвращает `200 OK` ответ.</span><span class="sxs-lookup"><span data-stu-id="5248d-131">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="5248d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5248d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5248d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5248d-133">Request</span></span>

<span data-ttu-id="5248d-134">Ниже приводится пример запроса на обновление свойства **policyViolation** в сообщении канала Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5248d-134">The following is an example of the request to update the **policyViolation** property on a Microsoft Teams channel message.</span></span>


# <a name="http"></a>[<span data-ttu-id="5248d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5248d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chatMessage.PatchPolicyViolation.All"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json
Content-Length: 248

{
  "policyViolation": {
    "policyTip": {
      "generalText" : "This item has been blocked by the administrator.",
      "complianceUrl" : "https://contoso.com/dlp-policy-page",
      "matchedConditionDescriptions" : ["Credit Card Number"]
    },
    "verdictDetails" : "AllowOverrideWithoutJustification,AllowFalsePositiveOverride",
    "dlpAction" : "BlockAccess"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="5248d-136">C#</span><span class="sxs-lookup"><span data-stu-id="5248d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chatmessagepatchpolicyviolationall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5248d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5248d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chatmessagepatchpolicyviolationall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5248d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5248d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chatmessagepatchpolicyviolationall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5248d-139">Java</span><span class="sxs-lookup"><span data-stu-id="5248d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chatmessagepatchpolicyviolationall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5248d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5248d-140">Response</span></span>

<span data-ttu-id="5248d-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5248d-141">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessage.UpdatePolicyViolation.All",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
