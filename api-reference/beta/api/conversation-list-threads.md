---
title: Список цепочек
description: Получение всех цепочек в групповой беседе.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: e1aacab39dfeae4dd9271ce5f3664c55eb80a583
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813309"
---
# <a name="list-threads"></a><span data-ttu-id="4d0d7-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="4d0d7-103">List threads</span></span>

> <span data-ttu-id="4d0d7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d0d7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d0d7-106">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-106">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="4d0d7-107">Примечание. Вы также можете [получить все цепочки группы](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="4d0d7-107">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="4d0d7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d0d7-108">Permissions</span></span>
<span data-ttu-id="4d0d7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d0d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d0d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d0d7-111">Permission type</span></span>      | <span data-ttu-id="4d0d7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d0d7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d0d7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d0d7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4d0d7-114">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d0d7-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="4d0d7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d0d7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d0d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-116">Not supported.</span></span>    |
|<span data-ttu-id="4d0d7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d0d7-117">Application</span></span> | <span data-ttu-id="4d0d7-118">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d0d7-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d0d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d0d7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4d0d7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d0d7-120">Optional query parameters</span></span>
<span data-ttu-id="4d0d7-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4d0d7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d0d7-122">Request headers</span></span>
| <span data-ttu-id="4d0d7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d0d7-123">Header</span></span>       | <span data-ttu-id="4d0d7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4d0d7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d0d7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d0d7-125">Authorization</span></span>  | <span data-ttu-id="4d0d7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d0d7-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d0d7-128">Request body</span></span>
<span data-ttu-id="4d0d7-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d0d7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d0d7-130">Response</span></span>

<span data-ttu-id="4d0d7-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d0d7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4d0d7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d0d7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d0d7-133">Request</span></span>
<span data-ttu-id="4d0d7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="4d0d7-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d0d7-135">Response</span></span>
<span data-ttu-id="4d0d7-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4d0d7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
