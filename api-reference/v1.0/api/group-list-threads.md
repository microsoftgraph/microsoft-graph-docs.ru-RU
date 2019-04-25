---
title: Список цепочек
description: Получение всех цепочек группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 860d9bc88aff010bbb8a563017474698f93535b9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550114"
---
# <a name="list-threads"></a><span data-ttu-id="28642-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="28642-103">List threads</span></span>
<span data-ttu-id="28642-104">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="28642-104">Get all the threads of a group.</span></span>

><span data-ttu-id="28642-105">Примечание. Вы также можете [получить все цепочки беседы](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="28642-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="28642-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28642-106">Permissions</span></span>
<span data-ttu-id="28642-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28642-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28642-109">Permission type</span></span>      | <span data-ttu-id="28642-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28642-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28642-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28642-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28642-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28642-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="28642-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28642-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28642-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28642-114">Not supported.</span></span>    |
|<span data-ttu-id="28642-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28642-115">Application</span></span> | <span data-ttu-id="28642-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28642-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28642-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28642-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28642-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="28642-118">Optional query parameters</span></span>
<span data-ttu-id="28642-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="28642-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28642-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28642-120">Request headers</span></span>
| <span data-ttu-id="28642-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28642-121">Header</span></span>       | <span data-ttu-id="28642-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28642-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28642-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28642-123">Authorization</span></span>  | <span data-ttu-id="28642-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28642-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28642-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28642-126">Request body</span></span>
<span data-ttu-id="28642-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28642-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28642-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="28642-128">Response</span></span>
<span data-ttu-id="28642-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ConversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28642-129">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28642-130">Пример</span><span class="sxs-lookup"><span data-stu-id="28642-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="28642-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="28642-131">Request</span></span>
<span data-ttu-id="28642-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28642-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="28642-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="28642-133">Response</span></span>
<span data-ttu-id="28642-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28642-134">The following is an example of the response.</span></span>
><span data-ttu-id="28642-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28642-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "lastDeliveredDateTime": "datetime-value",
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
