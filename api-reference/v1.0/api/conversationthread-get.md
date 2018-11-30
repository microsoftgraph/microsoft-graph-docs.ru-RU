---
title: Получение объекта conversationThread
description: 'Получение определенной цепочки, принадлежащей группе. Можно указать родительский беседы и поток, или, '
ms.openlocfilehash: 1c4e0da5a85464c07844c976140425a70fd48b76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026079"
---
# <a name="get-conversationthread"></a><span data-ttu-id="1e4b1-104">Получение объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="1e4b1-104">Get conversationThread</span></span>

<span data-ttu-id="1e4b1-p102">Получение определенной цепочки, принадлежащей группе. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="1e4b1-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="1e4b1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e4b1-107">Permissions</span></span>
<span data-ttu-id="1e4b1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e4b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e4b1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e4b1-110">Permission type</span></span>      | <span data-ttu-id="1e4b1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e4b1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e4b1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e4b1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e4b1-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e4b1-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="1e4b1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e4b1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e4b1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e4b1-115">Not supported.</span></span>    |
|<span data-ttu-id="1e4b1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e4b1-116">Application</span></span> | <span data-ttu-id="1e4b1-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e4b1-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e4b1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e4b1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e4b1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1e4b1-119">Optional query parameters</span></span>
<span data-ttu-id="1e4b1-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1e4b1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1e4b1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e4b1-121">Request headers</span></span>
| <span data-ttu-id="1e4b1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e4b1-122">Header</span></span>       | <span data-ttu-id="1e4b1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1e4b1-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e4b1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e4b1-124">Authorization</span></span>  | <span data-ttu-id="1e4b1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e4b1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e4b1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e4b1-127">Request body</span></span>
<span data-ttu-id="1e4b1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e4b1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e4b1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e4b1-129">Response</span></span>

<span data-ttu-id="1e4b1-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e4b1-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e4b1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1e4b1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e4b1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e4b1-132">Request</span></span>
<span data-ttu-id="1e4b1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e4b1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="1e4b1-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e4b1-134">Response</span></span>
<span data-ttu-id="1e4b1-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1e4b1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
