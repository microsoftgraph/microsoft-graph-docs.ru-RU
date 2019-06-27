---
title: Перечисление правил
description: Получение всех объектов messageRule, определенных для папки "Входящие" пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 031ab80ea28fc2bf711764e71513405935a515d9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266684"
---
# <a name="list-rules"></a><span data-ttu-id="be41c-103">Перечисление правил</span><span class="sxs-lookup"><span data-stu-id="be41c-103">List rules</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be41c-104">Получение всех объектов [messageRule](../resources/messagerule.md), определенных для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="be41c-104">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="be41c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be41c-105">Permissions</span></span>
<span data-ttu-id="be41c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be41c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be41c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be41c-108">Permission type</span></span>      | <span data-ttu-id="be41c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be41c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be41c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be41c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be41c-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="be41c-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="be41c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be41c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be41c-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="be41c-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="be41c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be41c-114">Application</span></span> | <span data-ttu-id="be41c-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="be41c-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="be41c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be41c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be41c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be41c-117">Optional query parameters</span></span>
<span data-ttu-id="be41c-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be41c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="be41c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be41c-119">Request headers</span></span>
| <span data-ttu-id="be41c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="be41c-120">Name</span></span>       | <span data-ttu-id="be41c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="be41c-121">Type</span></span> | <span data-ttu-id="be41c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="be41c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be41c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be41c-123">Authorization</span></span>  | <span data-ttu-id="be41c-124">string</span><span class="sxs-lookup"><span data-stu-id="be41c-124">string</span></span>  | <span data-ttu-id="be41c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be41c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be41c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be41c-127">Request body</span></span>
<span data-ttu-id="be41c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be41c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="be41c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="be41c-129">Response</span></span>
<span data-ttu-id="be41c-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="be41c-130">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be41c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="be41c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be41c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="be41c-132">Request</span></span>
<span data-ttu-id="be41c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be41c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
##### <a name="response"></a><span data-ttu-id="be41c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="be41c-134">Response</span></span>
<span data-ttu-id="be41c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be41c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="be41c-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="be41c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="be41c-139">C#</span><span class="sxs-lookup"><span data-stu-id="be41c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_messagerules-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be41c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="be41c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_messagerules-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="be41c-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="be41c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_messagerules-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailfolder-list-messagerules.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-messagerules.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-messagerules.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
