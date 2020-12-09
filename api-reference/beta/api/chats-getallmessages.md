---
title: 'чаты: getAllMessages'
description: Получение сообщений из всех чатах, в которых пользователь является участником.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cb23dd527a4f1bf78863602c1c8b01fa0e848b9d
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597767"
---
# <a name="chats-getallmessages"></a><span data-ttu-id="41e38-103">чаты: getAllMessages</span><span class="sxs-lookup"><span data-stu-id="41e38-103">chats: getAllMessages</span></span>

<span data-ttu-id="41e38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41e38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41e38-105">Получение всех сообщений ото всех [чатов](../resources/chatmessage.md), в которых пользователь является участником, включая чаты с одним участником, групповые чаты и чаты собраний.</span><span class="sxs-lookup"><span data-stu-id="41e38-105">Get all messages from all [chats](../resources/chatmessage.md) that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span>

## <a name="permissions"></a><span data-ttu-id="41e38-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41e38-106">Permissions</span></span>

<span data-ttu-id="41e38-107">Для вызова этого API требуются следующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="41e38-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="41e38-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41e38-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41e38-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41e38-109">Permission type</span></span>      | <span data-ttu-id="41e38-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41e38-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41e38-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41e38-111">Delegated (work or school account)</span></span>| <span data-ttu-id="41e38-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="41e38-112">Not supported</span></span> |
|<span data-ttu-id="41e38-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41e38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41e38-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="41e38-114">Not supported</span></span> |
|<span data-ttu-id="41e38-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="41e38-115">Application</span></span> | <span data-ttu-id="41e38-116">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41e38-116">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="41e38-117">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="41e38-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="41e38-118">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="41e38-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="41e38-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41e38-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/chats/getAllMessages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41e38-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="41e38-120">Optional query parameters</span></span>

<span data-ttu-id="41e38-121">Эта операция поддерживает [параметры диапазона дат](/graph/query-parameters) для настройки отклика, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="41e38-121">This operation supports [date range parameters](/graph/query-parameters) to customize the response, as shown in the following example.</span></span>

```http
GET /users/{id}/chats/getAllMessages?$top=50&$filter=lastModifiedDateTime gt 2020-06-04T18:03:11.591Z and lastModifiedDateTime lt 2020-06-05T21:00:09.413Z
```

## <a name="request-headers"></a><span data-ttu-id="41e38-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41e38-122">Request headers</span></span>
| <span data-ttu-id="41e38-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41e38-123">Header</span></span>       | <span data-ttu-id="41e38-124">Значение</span><span class="sxs-lookup"><span data-stu-id="41e38-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41e38-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41e38-125">Authorization</span></span>  | <span data-ttu-id="41e38-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41e38-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="41e38-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="41e38-128">Response</span></span>

<span data-ttu-id="41e38-129">В случае успеха этот метод возвращает `200 OK` код отклика и список [chatMessages](../resources/chatmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="41e38-129">If successful, this method returns a `200 OK` response code and a list of [chatMessages](../resources/chatmessage.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e38-130">Пример</span><span class="sxs-lookup"><span data-stu-id="41e38-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="41e38-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="41e38-131">Request</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages
```

### <a name="response"></a><span data-ttu-id="41e38-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="41e38-132">Response</span></span>

><span data-ttu-id="41e38-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="41e38-133">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK 
Content-type: application/json 
Content-length: 347 

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
   "@odata.count":10,
   "@odata.nextLink":"https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages?$skip=10",
   "value":[
      {
         "@odata.type":"#microsoft.graph.chatMessage",
         "id":"1600457965467",
         "replyToId":null,
         "etag":"1600457965467",
         "messageType":"message",
         "createdDateTime":"2020-09-18T19:39:25.467Z",
         "lastModifiedDateTime":"2020-09-18T19:39:25.467Z",
         "lastEditedDateTime":null,
         "deletedDateTime":null,
         "subject":null,
         "summary":null,
         "chatId":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_5c64e248-3269-4268-a36e-0f80314e9c39@unq.gbl.spaces",
         "importance":"normal",
         "locale":"en-us",
         "webUrl":null,
         "channelIdentity":null,
         "policyViolation":null,
         "from":{
            "application":null,
            "device":null,
            "conversation":null,
            "user":{
               "id":"0de69e5e-2da8-4cf2-821f-5e6585b2c65b",
               "displayName":"Richard Wilson",
               "userIdentityType":"aadUser"
            }
         },
         "body":{
            "contentType":"html",
            "content":"<div>\n<blockquote itemscope=\"\" itemtype=\"http://schema.skype.com/Reply\" itemid=\"1600457867820\">\n<strong itemprop=\"mri\" itemid=\"8:orgid:0de69e5e-2da8-4cf2-821f-5e6585b2c65b\">Richard Wilson</strong><span itemprop=\"time\" itemid=\"1600457867820\"></span>\n<p itemprop=\"preview\">1237</p>\n</blockquote>\n<p>this is a reply</p>\n</div>"
         },
         "attachments":[
            
         ],
         "mentions":[
            
         ],
         "reactions":[
            
         ]
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chats: getallmessages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
