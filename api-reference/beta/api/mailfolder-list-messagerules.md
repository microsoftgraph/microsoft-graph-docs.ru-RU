---
title: Перечисление правил
description: Получение всех объектов messageRule, определенных для папки "Входящие" пользователя.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9fa10dca78b917bf5662dd280e9b9cb60d4bff85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053617"
---
# <a name="list-rules"></a><span data-ttu-id="f72ce-103">Перечисление правил</span><span class="sxs-lookup"><span data-stu-id="f72ce-103">List rules</span></span>

<span data-ttu-id="f72ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f72ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f72ce-105">Получение всех объектов [messageRule](../resources/messagerule.md), определенных для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="f72ce-105">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="f72ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f72ce-106">Permissions</span></span>
<span data-ttu-id="f72ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f72ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f72ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f72ce-109">Permission type</span></span>      | <span data-ttu-id="f72ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f72ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f72ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f72ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f72ce-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="f72ce-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="f72ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f72ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f72ce-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="f72ce-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="f72ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f72ce-115">Application</span></span> | <span data-ttu-id="f72ce-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="f72ce-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f72ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f72ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f72ce-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f72ce-118">Optional query parameters</span></span>
<span data-ttu-id="f72ce-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f72ce-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f72ce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f72ce-120">Request headers</span></span>
| <span data-ttu-id="f72ce-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f72ce-121">Name</span></span>       | <span data-ttu-id="f72ce-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f72ce-122">Type</span></span> | <span data-ttu-id="f72ce-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f72ce-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f72ce-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f72ce-124">Authorization</span></span>  | <span data-ttu-id="f72ce-125">string</span><span class="sxs-lookup"><span data-stu-id="f72ce-125">string</span></span>  | <span data-ttu-id="f72ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f72ce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f72ce-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f72ce-128">Request body</span></span>
<span data-ttu-id="f72ce-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f72ce-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f72ce-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f72ce-130">Response</span></span>
<span data-ttu-id="f72ce-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f72ce-131">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f72ce-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f72ce-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f72ce-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f72ce-133">Request</span></span>
<span data-ttu-id="f72ce-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f72ce-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f72ce-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f72ce-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
# <a name="c"></a>[<span data-ttu-id="f72ce-136">C#</span><span class="sxs-lookup"><span data-stu-id="f72ce-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f72ce-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f72ce-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f72ce-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f72ce-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f72ce-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f72ce-139">Response</span></span>
<span data-ttu-id="f72ce-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f72ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


