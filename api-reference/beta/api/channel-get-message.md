---
title: Сообщение канала
description: Получение единственного сообщения (без его ответы) в канале команды.
author: nkramer
ms.openlocfilehash: 2da10f4151cc1ddaaa1bddfe376f4035a6baa180
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309228"
---
# <a name="get-channel-message"></a><span data-ttu-id="dc669-103">Сообщение канала</span><span class="sxs-lookup"><span data-stu-id="dc669-103">Get channel message</span></span>

> <span data-ttu-id="dc669-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc669-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc669-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc669-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc669-106">Получение единственного [сообщения](../resources/chatmessage.md) (без его ответы) в [канал](../resources/channel.md) группы.</span><span class="sxs-lookup"><span data-stu-id="dc669-106">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc669-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc669-107">Permissions</span></span>
<span data-ttu-id="dc669-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc669-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc669-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc669-110">Permission Type</span></span>|<span data-ttu-id="dc669-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc669-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="dc669-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc669-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc669-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc669-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="dc669-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc669-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc669-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc669-115">Not supported</span></span>|
|<span data-ttu-id="dc669-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc669-116">Application</span></span>| <span data-ttu-id="dc669-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc669-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc669-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc669-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc669-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dc669-119">Optional query parameters</span></span>
<span data-ttu-id="dc669-120">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="dc669-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc669-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc669-121">Request headers</span></span>
| <span data-ttu-id="dc669-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc669-122">Header</span></span>       | <span data-ttu-id="dc669-123">Значение</span><span class="sxs-lookup"><span data-stu-id="dc669-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc669-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc669-124">Authorization</span></span>  | <span data-ttu-id="dc669-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc669-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc669-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc669-127">Request body</span></span>
<span data-ttu-id="dc669-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc669-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc669-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc669-129">Response</span></span>

<span data-ttu-id="dc669-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [chatmessage](../resources/chatmessage.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dc669-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc669-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dc669-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc669-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc669-132">Request</span></span>
<span data-ttu-id="dc669-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc669-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="dc669-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc669-134">Response</span></span>
<span data-ttu-id="dc669-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc669-135">Here is an example of the response.</span></span> 

><span data-ttu-id="dc669-136">**Примечание:** Объект ответа, показанный сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="dc669-136">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="dc669-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc669-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "replyToId": "id-value",
  "from": {
      "user": { 
        "id": "id-value",
        "displayName": "John Doe"
      }  
  },
  "etag": "id-value",
  "messageType": "message",
  "createdDateTime": "2018-07-09T07:40:20.152Z",
  "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
  "body": {
      "content": "Hello World",
      "contentType": "text"
  },
  "attachments": [
        {
            "id": "5e32f195-168a-474f-a273-123123123",
            "contentType": "reference",
            "contentUrl": "https://test.sharepoint.com/sites/TestSite/Shared%20Documents/General/Test.txt",
            "content": null,
            "name": "Test.txt",
            "thumbnailUrl": null
        }
  ],
  "mentions": [
      {
          "type": "user",
          "id": "id-value ",
          "mentionText": "Test User"
      }
  ],
  "importance": "normal",
  "reactions": [
      {
        "reactionType": "like",
        "user": {
            "id": "id-value",
            "displayName": "John Doe"
        },
        "createdDateTime": "2018-07-09T07:40:20.152Z"
      }
  ],
  "locale": "en-us"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
