---
title: Список сообщений
description: Получение всех сообщений в почтовом ящике вошедшего пользователя или в указанной папке этого почтового ящика.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0c3aca6f718548155a5a13ff617dacfa61f54927
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511630"
---
# <a name="list-messages"></a><span data-ttu-id="49375-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="49375-103">List messages</span></span>

<span data-ttu-id="49375-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49375-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49375-105">Получение всех сообщений в почтовом ящике определенного пользователя или в указанной папке этого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="49375-105">Get all the messages in the specified user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="49375-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49375-106">Permissions</span></span>
<span data-ttu-id="49375-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49375-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49375-109">Permission type</span></span>      | <span data-ttu-id="49375-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49375-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49375-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49375-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49375-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49375-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="49375-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49375-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49375-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49375-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="49375-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="49375-115">Application</span></span> | <span data-ttu-id="49375-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49375-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="49375-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49375-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49375-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49375-118">Optional query parameters</span></span>
<span data-ttu-id="49375-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="49375-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="49375-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49375-120">Request headers</span></span>
| <span data-ttu-id="49375-121">Имя</span><span class="sxs-lookup"><span data-stu-id="49375-121">Name</span></span>       | <span data-ttu-id="49375-122">Тип</span><span class="sxs-lookup"><span data-stu-id="49375-122">Type</span></span> | <span data-ttu-id="49375-123">Описание</span><span class="sxs-lookup"><span data-stu-id="49375-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="49375-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="49375-124">Authorization</span></span>  | <span data-ttu-id="49375-125">string</span><span class="sxs-lookup"><span data-stu-id="49375-125">string</span></span>  | <span data-ttu-id="49375-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49375-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49375-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49375-128">Request body</span></span>
<span data-ttu-id="49375-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49375-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49375-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="49375-130">Response</span></span>

<span data-ttu-id="49375-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49375-131">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49375-132">Пример</span><span class="sxs-lookup"><span data-stu-id="49375-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49375-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="49375-133">Request</span></span>
<span data-ttu-id="49375-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49375-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49375-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="49375-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
# <a name="c"></a>[<span data-ttu-id="49375-136">C#</span><span class="sxs-lookup"><span data-stu-id="49375-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49375-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49375-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49375-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49375-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49375-139">Java</span><span class="sxs-lookup"><span data-stu-id="49375-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49375-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="49375-140">Response</span></span>
<span data-ttu-id="49375-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49375-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
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
