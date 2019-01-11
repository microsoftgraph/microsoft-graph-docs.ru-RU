---
title: Список цепочек
description: Получение всех цепочек группы.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: a15c9def749717f7134bc0a34cac868e0bc10897
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870471"
---
# <a name="list-threads"></a><span data-ttu-id="62a95-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="62a95-103">List threads</span></span>

> <span data-ttu-id="62a95-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62a95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62a95-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62a95-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="62a95-106">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="62a95-106">Get all the threads of a group.</span></span>

<span data-ttu-id="62a95-107">Примечание. Вы также можете [получить все цепочки беседы](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="62a95-107">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="62a95-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62a95-108">Permissions</span></span>
<span data-ttu-id="62a95-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62a95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62a95-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62a95-111">Permission type</span></span>      | <span data-ttu-id="62a95-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62a95-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62a95-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62a95-113">Delegated (work or school account)</span></span> | <span data-ttu-id="62a95-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a95-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="62a95-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62a95-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62a95-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62a95-116">Not supported.</span></span>    |
|<span data-ttu-id="62a95-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62a95-117">Application</span></span> | <span data-ttu-id="62a95-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62a95-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62a95-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62a95-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62a95-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62a95-120">Optional query parameters</span></span>
<span data-ttu-id="62a95-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="62a95-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62a95-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62a95-122">Request headers</span></span>
| <span data-ttu-id="62a95-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62a95-123">Header</span></span>       | <span data-ttu-id="62a95-124">Значение</span><span class="sxs-lookup"><span data-stu-id="62a95-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="62a95-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62a95-125">Authorization</span></span>  | <span data-ttu-id="62a95-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62a95-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="62a95-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62a95-128">Request body</span></span>
<span data-ttu-id="62a95-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62a95-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62a95-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="62a95-130">Response</span></span>
<span data-ttu-id="62a95-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62a95-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62a95-132">Пример</span><span class="sxs-lookup"><span data-stu-id="62a95-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="62a95-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="62a95-133">Request</span></span>
<span data-ttu-id="62a95-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62a95-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="62a95-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="62a95-135">Response</span></span>
<span data-ttu-id="62a95-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="62a95-136">The following is an example of the response.</span></span>
><span data-ttu-id="62a95-137">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="62a95-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="62a95-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62a95-138">All the properties will be returned from an actual call.</span></span>
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
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
