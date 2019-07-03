---
title: Список сообщений
description: Получение всех сообщений в почтовом ящике вошедшего пользователя или в указанной папке этого почтового ящика.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: a15b129c8a2204037796b17c26598eb433453310
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454379"
---
# <a name="list-messages"></a><span data-ttu-id="6451d-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="6451d-103">List messages</span></span>

<span data-ttu-id="6451d-104">Получение всех сообщений в почтовом ящике определенного пользователя или в указанной папке этого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6451d-104">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="6451d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6451d-105">Permissions</span></span>
<span data-ttu-id="6451d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6451d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6451d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6451d-108">Permission type</span></span>      | <span data-ttu-id="6451d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6451d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6451d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6451d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6451d-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6451d-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6451d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6451d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6451d-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6451d-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6451d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6451d-114">Application</span></span> | <span data-ttu-id="6451d-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6451d-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6451d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6451d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6451d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6451d-117">Optional query parameters</span></span>
<span data-ttu-id="6451d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6451d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6451d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6451d-119">Request headers</span></span>
| <span data-ttu-id="6451d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6451d-120">Name</span></span>       | <span data-ttu-id="6451d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6451d-121">Type</span></span> | <span data-ttu-id="6451d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6451d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6451d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6451d-123">Authorization</span></span>  | <span data-ttu-id="6451d-124">string</span><span class="sxs-lookup"><span data-stu-id="6451d-124">string</span></span>  | <span data-ttu-id="6451d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6451d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6451d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6451d-127">Request body</span></span>
<span data-ttu-id="6451d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6451d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6451d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6451d-129">Response</span></span>

<span data-ttu-id="6451d-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6451d-130">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6451d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6451d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6451d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6451d-132">Request</span></span>
<span data-ttu-id="6451d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6451d-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6451d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6451d-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6451d-135">C#</span><span class="sxs-lookup"><span data-stu-id="6451d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6451d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6451d-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6451d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6451d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6451d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6451d-138">Response</span></span>
<span data-ttu-id="6451d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6451d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
