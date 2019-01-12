---
title: Получение объекта conversationThread
description: 'Получение определенной цепочки, принадлежащей группе. Можно указать родительский беседы и поток, или, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 25889fad4dc60cbd69ee4e87ca8a7f4406f9e6f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935754"
---
# <a name="get-conversationthread"></a><span data-ttu-id="d1e53-104">Получение объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="d1e53-104">Get conversationThread</span></span>

> <span data-ttu-id="d1e53-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d1e53-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1e53-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1e53-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1e53-p103">Получение определенной цепочки, принадлежащей группе. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="d1e53-p103">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="d1e53-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1e53-109">Permissions</span></span>
<span data-ttu-id="d1e53-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1e53-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1e53-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1e53-112">Permission type</span></span>      | <span data-ttu-id="d1e53-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1e53-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1e53-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1e53-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d1e53-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1e53-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="d1e53-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1e53-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1e53-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1e53-117">Not supported.</span></span>    |
|<span data-ttu-id="d1e53-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1e53-118">Application</span></span> | <span data-ttu-id="d1e53-119">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1e53-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1e53-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1e53-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1e53-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1e53-121">Optional query parameters</span></span>
<span data-ttu-id="d1e53-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d1e53-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d1e53-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1e53-123">Request headers</span></span>
| <span data-ttu-id="d1e53-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1e53-124">Header</span></span>       | <span data-ttu-id="d1e53-125">Значение</span><span class="sxs-lookup"><span data-stu-id="d1e53-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1e53-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1e53-126">Authorization</span></span>  | <span data-ttu-id="d1e53-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1e53-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1e53-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1e53-129">Request body</span></span>
<span data-ttu-id="d1e53-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1e53-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1e53-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1e53-131">Response</span></span>

<span data-ttu-id="d1e53-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1e53-132">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1e53-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d1e53-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1e53-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1e53-134">Request</span></span>
<span data-ttu-id="d1e53-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1e53-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="d1e53-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1e53-136">Response</span></span>
<span data-ttu-id="d1e53-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d1e53-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
