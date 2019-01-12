---
title: Перечисление правил
description: Получение всех объектов messageRule, определенных для папки "Входящие" пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d5c0dea2844c62133a15a4463cd2ea473f310a37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951231"
---
# <a name="list-rules"></a><span data-ttu-id="910fc-103">Перечисление правил</span><span class="sxs-lookup"><span data-stu-id="910fc-103">List rules</span></span>

> <span data-ttu-id="910fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="910fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="910fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="910fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="910fc-106">Получение всех объектов [messageRule](../resources/messagerule.md), определенных для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="910fc-106">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="910fc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="910fc-107">Permissions</span></span>
<span data-ttu-id="910fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="910fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="910fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="910fc-110">Permission type</span></span>      | <span data-ttu-id="910fc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="910fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="910fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="910fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="910fc-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="910fc-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="910fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="910fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="910fc-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="910fc-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="910fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="910fc-116">Application</span></span> | <span data-ttu-id="910fc-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="910fc-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="910fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="910fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="910fc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="910fc-119">Optional query parameters</span></span>
<span data-ttu-id="910fc-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="910fc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="910fc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="910fc-121">Request headers</span></span>
| <span data-ttu-id="910fc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="910fc-122">Name</span></span>       | <span data-ttu-id="910fc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="910fc-123">Type</span></span> | <span data-ttu-id="910fc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="910fc-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="910fc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="910fc-125">Authorization</span></span>  | <span data-ttu-id="910fc-126">string</span><span class="sxs-lookup"><span data-stu-id="910fc-126">string</span></span>  | <span data-ttu-id="910fc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="910fc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="910fc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="910fc-129">Request body</span></span>
<span data-ttu-id="910fc-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="910fc-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="910fc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="910fc-131">Response</span></span>
<span data-ttu-id="910fc-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="910fc-132">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="910fc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="910fc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="910fc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="910fc-134">Request</span></span>
<span data-ttu-id="910fc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="910fc-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
##### <a name="response"></a><span data-ttu-id="910fc-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="910fc-136">Response</span></span>
<span data-ttu-id="910fc-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="910fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
