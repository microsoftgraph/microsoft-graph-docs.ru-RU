---
title: Список цепочек
description: Получение всех цепочек группы.
ms.openlocfilehash: 659d80793f2ad4ededaabca7087f470c0cc6c081
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028255"
---
# <a name="list-threads"></a><span data-ttu-id="8df8d-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="8df8d-103">List threads</span></span>
<span data-ttu-id="8df8d-104">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="8df8d-104">Get all the threads of a group.</span></span>

><span data-ttu-id="8df8d-105">Примечание. Вы также можете [получить все цепочки беседы](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="8df8d-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8df8d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8df8d-106">Permissions</span></span>
<span data-ttu-id="8df8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8df8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df8d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8df8d-109">Permission type</span></span>      | <span data-ttu-id="8df8d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8df8d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8df8d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8df8d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8df8d-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df8d-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8df8d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8df8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8df8d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df8d-114">Not supported.</span></span>    |
|<span data-ttu-id="8df8d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8df8d-115">Application</span></span> | <span data-ttu-id="8df8d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df8d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8df8d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8df8d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8df8d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8df8d-118">Optional query parameters</span></span>
<span data-ttu-id="8df8d-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8df8d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8df8d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8df8d-120">Request headers</span></span>
| <span data-ttu-id="8df8d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8df8d-121">Header</span></span>       | <span data-ttu-id="8df8d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8df8d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8df8d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8df8d-123">Authorization</span></span>  | <span data-ttu-id="8df8d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8df8d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8df8d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8df8d-126">Request body</span></span>
<span data-ttu-id="8df8d-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8df8d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8df8d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8df8d-128">Response</span></span>
<span data-ttu-id="8df8d-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ConversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8df8d-129">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df8d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8df8d-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8df8d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8df8d-131">Request</span></span>
<span data-ttu-id="8df8d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8df8d-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="8df8d-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="8df8d-133">Response</span></span>
<span data-ttu-id="8df8d-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8df8d-134">The following is an example of the response.</span></span>
><span data-ttu-id="8df8d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8df8d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
