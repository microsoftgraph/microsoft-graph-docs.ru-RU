---
title: Создание объекта chatMessage в канале
description: Создание нового chatMessage в указанном канале.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e80eab3d3935c119046570576a18344447a486d8
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192361"
---
# <a name="create-chatmessage-in-channel"></a><span data-ttu-id="85356-103">Создание chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="85356-103">Create chatMessage in channel</span></span>

<span data-ttu-id="85356-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85356-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85356-105">Создание нового [chatMessage](../resources/chatmessage.md) в указанном [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="85356-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="85356-106">**Note**: мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="85356-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="85356-107">Пропускная способность, необходимая для обычной миграции, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="85356-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="85356-108">**Note**: нарушение [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) Microsoft Teams в качестве файла журнала.</span><span class="sxs-lookup"><span data-stu-id="85356-108">**Note**: It is a violation of the [terms of use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="85356-109">Отправлять только сообщения, которые пользователи смогут читать.</span><span class="sxs-lookup"><span data-stu-id="85356-109">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="85356-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85356-110">Permissions</span></span>

<span data-ttu-id="85356-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85356-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85356-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85356-113">Permission type</span></span>                        | <span data-ttu-id="85356-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85356-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85356-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85356-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="85356-116">Чаннелмессаже. Send, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="85356-116">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="85356-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85356-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85356-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85356-118">Not supported.</span></span> |
| <span data-ttu-id="85356-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85356-119">Application</span></span>                            | <span data-ttu-id="85356-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85356-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85356-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85356-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="85356-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85356-122">Request headers</span></span>

| <span data-ttu-id="85356-123">Имя</span><span class="sxs-lookup"><span data-stu-id="85356-123">Name</span></span>          | <span data-ttu-id="85356-124">Описание</span><span class="sxs-lookup"><span data-stu-id="85356-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="85356-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85356-125">Authorization</span></span> | <span data-ttu-id="85356-126">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="85356-126">Bearer {code}.</span></span> <span data-ttu-id="85356-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="85356-127">Required.</span></span> |
| <span data-ttu-id="85356-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85356-128">Content-type</span></span> | <span data-ttu-id="85356-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85356-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85356-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85356-131">Request body</span></span>

<span data-ttu-id="85356-132">В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85356-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="85356-133">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="85356-133">Only the body property is mandatory, other properties are optional.</span></span>


## <a name="response"></a><span data-ttu-id="85356-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="85356-134">Response</span></span>

<span data-ttu-id="85356-135">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85356-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85356-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="85356-136">Examples</span></span>

<span data-ttu-id="85356-137">Более полный список примеров приведен [в статье Создание chatMessage в канале или чате](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="85356-137">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="85356-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="85356-138">Request</span></span>
<span data-ttu-id="85356-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85356-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85356-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="85356-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="85356-141">C#</span><span class="sxs-lookup"><span data-stu-id="85356-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85356-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85356-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85356-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85356-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85356-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="85356-144">Response</span></span>

<span data-ttu-id="85356-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85356-145">The following is an example of the response.</span></span>

> <span data-ttu-id="85356-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85356-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


