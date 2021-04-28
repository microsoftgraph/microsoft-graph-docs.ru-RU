---
title: Список сообщений
description: Получение всех сообщений в почтовом ящике вошедшего пользователя или в указанной папке этого почтового ящика.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 34b3dd40698b92f7e7726952fd404dfd45415fae
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049515"
---
# <a name="list-messages"></a><span data-ttu-id="be4f2-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="be4f2-103">List messages</span></span>

<span data-ttu-id="be4f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be4f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="be4f2-105">Получение всех сообщений в почтовом ящике определенного пользователя или в указанной папке этого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="be4f2-105">Get all the messages in the specified user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="be4f2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be4f2-106">Permissions</span></span>
<span data-ttu-id="be4f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be4f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be4f2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be4f2-109">Permission type</span></span>      | <span data-ttu-id="be4f2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be4f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be4f2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be4f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="be4f2-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be4f2-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="be4f2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be4f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be4f2-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be4f2-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="be4f2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="be4f2-115">Application</span></span> | <span data-ttu-id="be4f2-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be4f2-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="be4f2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be4f2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be4f2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be4f2-118">Optional query parameters</span></span>
<span data-ttu-id="be4f2-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be4f2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="be4f2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be4f2-120">Request headers</span></span>
| <span data-ttu-id="be4f2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="be4f2-121">Name</span></span>       | <span data-ttu-id="be4f2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="be4f2-122">Type</span></span> | <span data-ttu-id="be4f2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="be4f2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be4f2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="be4f2-124">Authorization</span></span>  | <span data-ttu-id="be4f2-125">string</span><span class="sxs-lookup"><span data-stu-id="be4f2-125">string</span></span>  | <span data-ttu-id="be4f2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be4f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be4f2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be4f2-128">Request body</span></span>
<span data-ttu-id="be4f2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be4f2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be4f2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="be4f2-130">Response</span></span>

<span data-ttu-id="be4f2-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be4f2-131">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be4f2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="be4f2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be4f2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="be4f2-133">Request</span></span>
<span data-ttu-id="be4f2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be4f2-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be4f2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="be4f2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
# <a name="c"></a>[<span data-ttu-id="be4f2-136">C#</span><span class="sxs-lookup"><span data-stu-id="be4f2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be4f2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be4f2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be4f2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be4f2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be4f2-139">Java</span><span class="sxs-lookup"><span data-stu-id="be4f2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="be4f2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="be4f2-140">Response</span></span>
<span data-ttu-id="be4f2-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be4f2-141">Here is an example of the response.</span></span> <span data-ttu-id="be4f2-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="be4f2-142">Note: The response object shown here might be shortened for readability.</span></span>
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
      "receivedDateTime": "2018-02-13T03:53:55Z",
      "sentDateTime": "2018-02-13T03:53:55Z",
      "hasAttachments": true,
      "subject": "MyAnalytics | Your past week",
      "body": {
        "contentType": "html",
        "content": "<html lang=\"en\">\r\n<head></head>\r\n<body> </body>\r\n</html>\r\n"
      },
      "bodyPreview": "February 4-10, 2018\r\n\r\n\r\nHi Megan Bowen,\r\n\r\nWe've got your highlights from last week\r\n\r\n\r\n\r\nYour time\r\n\r\n\r\nEmail hours\r\n\r\n\r\n\r\n\r\n0 hrs\r\n\r\n\r\n\r\nMeeting hours\r\n\r\n\r\n\r\n\r\n12 hrs\r\n\r\n\r\n\r\n\r\nFocus hours\r\n\r\n\r\n\r\n\r\n30 hrs\r\n\r\n\r\n\r\n\r\n\r\nGoals keep you motivated. Set them"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
