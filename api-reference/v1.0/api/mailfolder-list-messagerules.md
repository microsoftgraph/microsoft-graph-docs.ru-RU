---
title: Перечисление правил
description: Получение всех объектов messageRule, определенных для папки "Входящие" пользователя.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bae5c9658fe3f0036ba8682ec08d42e095935856
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402095"
---
# <a name="list-rules"></a><span data-ttu-id="6c777-103">Перечисление правил</span><span class="sxs-lookup"><span data-stu-id="6c777-103">List rules</span></span>

<span data-ttu-id="6c777-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c777-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c777-105">Получение всех объектов [messageRule](../resources/messagerule.md), определенных для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="6c777-105">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c777-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c777-106">Permissions</span></span>
<span data-ttu-id="6c777-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c777-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c777-109">Permission type</span></span>      | <span data-ttu-id="6c777-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c777-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c777-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c777-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6c777-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="6c777-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="6c777-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c777-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c777-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="6c777-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="6c777-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c777-115">Application</span></span> | <span data-ttu-id="6c777-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="6c777-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c777-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c777-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6c777-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6c777-118">Optional query parameters</span></span>
<span data-ttu-id="6c777-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6c777-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6c777-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c777-120">Request headers</span></span>
| <span data-ttu-id="6c777-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6c777-121">Name</span></span>       | <span data-ttu-id="6c777-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6c777-122">Type</span></span> | <span data-ttu-id="6c777-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6c777-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6c777-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c777-124">Authorization</span></span>  | <span data-ttu-id="6c777-125">string</span><span class="sxs-lookup"><span data-stu-id="6c777-125">string</span></span>  | <span data-ttu-id="6c777-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c777-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c777-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c777-128">Request body</span></span>
<span data-ttu-id="6c777-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c777-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6c777-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c777-130">Response</span></span>
<span data-ttu-id="6c777-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6c777-131">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c777-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6c777-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c777-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c777-133">Request</span></span>
<span data-ttu-id="6c777-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c777-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c777-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c777-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "get_messagerules"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
```
# <a name="c"></a>[<span data-ttu-id="6c777-136">C#</span><span class="sxs-lookup"><span data-stu-id="6c777-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c777-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c777-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c777-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c777-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c777-139">Java</span><span class="sxs-lookup"><span data-stu-id="6c777-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6c777-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c777-140">Response</span></span>
<span data-ttu-id="6c777-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c777-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules",
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
<!-- {
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->