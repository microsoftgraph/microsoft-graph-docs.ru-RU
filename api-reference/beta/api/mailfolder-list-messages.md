---
title: Список сообщений
description: Список всех сообщений в почтовом ящике вошедшего пользователя или сообщений в указанной папке почтового ящика или диска.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4f19b214d1e73b3809f8ea905b9ee561476250e6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44894881"
---
# <a name="list-messages"></a><span data-ttu-id="77235-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="77235-103">List messages</span></span>

<span data-ttu-id="77235-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77235-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77235-105">Список всех сообщений в почтовом ящике указанного пользователя или сообщений в указанной папке почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="77235-105">List all the messages in the specified user's mailbox, or those messages in a specified folder in the mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="77235-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77235-106">Permissions</span></span>
<span data-ttu-id="77235-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="77235-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="77235-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77235-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77235-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77235-109">Permission type</span></span>      | <span data-ttu-id="77235-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77235-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77235-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77235-111">Delegated (work or school account)</span></span> | <span data-ttu-id="77235-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77235-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="77235-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77235-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77235-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77235-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="77235-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="77235-115">Application</span></span> | <span data-ttu-id="77235-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77235-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="77235-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77235-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77235-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77235-118">Optional query parameters</span></span>
<span data-ttu-id="77235-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77235-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77235-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77235-120">Request headers</span></span>
| <span data-ttu-id="77235-121">Имя</span><span class="sxs-lookup"><span data-stu-id="77235-121">Name</span></span>       | <span data-ttu-id="77235-122">Тип</span><span class="sxs-lookup"><span data-stu-id="77235-122">Type</span></span> | <span data-ttu-id="77235-123">Описание</span><span class="sxs-lookup"><span data-stu-id="77235-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="77235-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77235-124">Authorization</span></span>  | <span data-ttu-id="77235-125">string</span><span class="sxs-lookup"><span data-stu-id="77235-125">string</span></span>  | <span data-ttu-id="77235-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="77235-126">Bearer {token}.</span></span> <span data-ttu-id="77235-127">Required.</span><span class="sxs-lookup"><span data-stu-id="77235-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77235-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77235-128">Request body</span></span>
<span data-ttu-id="77235-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77235-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77235-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="77235-130">Response</span></span>
<span data-ttu-id="77235-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77235-131">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77235-132">Пример</span><span class="sxs-lookup"><span data-stu-id="77235-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="77235-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="77235-133">Request</span></span>
<span data-ttu-id="77235-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77235-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77235-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="77235-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/messages
```
# <a name="c"></a>[<span data-ttu-id="77235-136">C#</span><span class="sxs-lookup"><span data-stu-id="77235-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77235-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77235-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77235-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77235-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="77235-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="77235-139">Response</span></span>
<span data-ttu-id="77235-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77235-140">The following is an example of the response.</span></span>
><span data-ttu-id="77235-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="77235-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="77235-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77235-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "id": "AAMkAGVmMDEzK",
      "createdDateTime": "2018-02-13T03:53:55Z",
      "lastModifiedDateTime": "2018-02-13T03:53:55Z",
      "changeKey": "CQAAABYAAAAiIsqMbYjsT5e/T7KzowPTAACB/CZh",
      "categories": [],
      "receivedDateTime": "2018-02-13T03:53:55Z",
      "sentDateTime": "2018-02-13T03:53:55Z",
      "hasAttachments": false,
      "internetMessageId": "<DM5PR1501MB2117E943C78792608769840ECDF60@DM5PR1501MB2117.namprd15.prod.outlook.com>",
      "subject": "MyAnalytics | Your past week",
      "bodyPreview": "February 4-10, 2018\r\n\r\n\r\nHi Megan Bowen,\r\n\r\nWe've got your highlights from last week\r\n\r\n\r\n\r\nYour time\r\n\r\n\r\nEmail hours\r\n\r\n\r\n\r\n\r\n0 hrs\r\n\r\n\r\n\r\nMeeting hours\r\n\r\n\r\n\r\n\r\n12 hrs\r\n\r\n\r\n\r\n\r\nFocus hours\r\n\r\n\r\n\r\n\r\n30 hrs\r\n\r\n\r\n\r\n\r\n\r\nGoals keep you motivated. Set them",
      "importance": "normal",
      "parentFolderId": "AAMkAGVmMDEzM",
      "conversationId": "AAQkAGVmMDEzE",
      "conversationIndex": "AQHTpH5EZfLlhf/DnUK56FDP+qUfcQ==",
      "isDeliveryReceiptRequested": false,
      "isReadReceiptRequested": false,
      "isRead": false,
      "isDraft": false,
      "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkAGVmMDEzK&exvsurl=1&viewmodel=ReadMessageItem",
      "inferenceClassification": "other",
      "unsubscribeData": [],
      "unsubscribeEnabled": false,
      "body": {
          "contentType": "html",
          "content": "<html lang=\"en\">\r\n<head></head>\r\n<body> </body>\r\n</html>\r\n"
      },
      "sender": {
          "emailAddress": {
              "name": "MyAnalytics",
              "address": "no-reply@microsoft.com"
          }
      },
      "from": {
          "emailAddress": {
              "name": "MyAnalytics",
              "address": "no-reply@microsoft.com"
          }
      },
      "toRecipients": [
          {
              "emailAddress": {
                  "name": "Megan Bowen",
                  "address": "MeganB@M365x214355.onmicrosoft.com"
              }
          }
      ],
      "ccRecipients": [],
      "bccRecipients": [],
      "replyTo": [],
      "mentionsPreview": null,
      "flag": {
          "flagStatus": "notFlagged"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
