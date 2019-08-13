---
title: Перечисление правил
description: Получение всех объектов messageRule, определенных для папки "Входящие" пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: aa441b6c519d9d7e78e39b1ef97731190df8580e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342873"
---
# <a name="list-rules"></a><span data-ttu-id="73943-103">Перечисление правил</span><span class="sxs-lookup"><span data-stu-id="73943-103">List rules</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73943-104">Получение всех объектов [messageRule](../resources/messagerule.md), определенных для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="73943-104">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="73943-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73943-105">Permissions</span></span>
<span data-ttu-id="73943-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73943-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73943-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73943-108">Permission type</span></span>      | <span data-ttu-id="73943-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73943-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73943-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73943-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73943-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="73943-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="73943-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73943-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73943-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="73943-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="73943-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73943-114">Application</span></span> | <span data-ttu-id="73943-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="73943-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="73943-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73943-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73943-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73943-117">Optional query parameters</span></span>
<span data-ttu-id="73943-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="73943-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="73943-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73943-119">Request headers</span></span>
| <span data-ttu-id="73943-120">Имя</span><span class="sxs-lookup"><span data-stu-id="73943-120">Name</span></span>       | <span data-ttu-id="73943-121">Тип</span><span class="sxs-lookup"><span data-stu-id="73943-121">Type</span></span> | <span data-ttu-id="73943-122">Описание</span><span class="sxs-lookup"><span data-stu-id="73943-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73943-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73943-123">Authorization</span></span>  | <span data-ttu-id="73943-124">string</span><span class="sxs-lookup"><span data-stu-id="73943-124">string</span></span>  | <span data-ttu-id="73943-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73943-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73943-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73943-127">Request body</span></span>
<span data-ttu-id="73943-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73943-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="73943-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="73943-129">Response</span></span>
<span data-ttu-id="73943-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="73943-130">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73943-131">Пример</span><span class="sxs-lookup"><span data-stu-id="73943-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73943-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="73943-132">Request</span></span>
<span data-ttu-id="73943-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73943-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73943-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="73943-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73943-135">C#</span><span class="sxs-lookup"><span data-stu-id="73943-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73943-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73943-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73943-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="73943-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73943-138">Java</span><span class="sxs-lookup"><span data-stu-id="73943-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="73943-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="73943-139">Response</span></span>
<span data-ttu-id="73943-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73943-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules",
  "value":[
    {
      "id":"AQAAAJ5dZp8=",
      "displayName":"Remove spam",
      "sequence":1,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "subjectContains":[
          "enter to win"
        ]
      },
      "actions":{
        "delete":true,
        "stopProcessingRules":true
      }
    },
    {
      "id":"AQAAAJ5dZqA=",
      "displayName":"From partner",
      "sequence":2,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "senderContains":[
          "ADELE"
        ]
      },
      "actions":{
        "stopProcessingRules":true,
        "forwardTo":[
          {
            "emailAddress":{
              "name":"Alex Wilbur",
              "address":"AlexW@contoso.onmicrosoft.com"
            }
          }
        ]
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
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
