---
title: Получение объекта conversationThread
description: 'Получение определенной цепочки, принадлежащей группе. Вы можете указать родительский сеанс связи и поток, или '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c89ed29d6cbdf4f392656d853ac41efc9964a5c4
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405500"
---
# <a name="get-conversationthread"></a><span data-ttu-id="ec9cd-104">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="ec9cd-104">Get conversationThread</span></span>

<span data-ttu-id="ec9cd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec9cd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec9cd-p102">Получение определенной цепочки, принадлежащей группе. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="ec9cd-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="ec9cd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec9cd-108">Permissions</span></span>
<span data-ttu-id="ec9cd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec9cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec9cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec9cd-111">Permission type</span></span>      | <span data-ttu-id="ec9cd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec9cd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec9cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec9cd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ec9cd-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec9cd-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ec9cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec9cd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec9cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec9cd-116">Not supported.</span></span>    |
|<span data-ttu-id="ec9cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec9cd-117">Application</span></span> | <span data-ttu-id="ec9cd-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec9cd-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec9cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec9cd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec9cd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec9cd-120">Optional query parameters</span></span>
<span data-ttu-id="ec9cd-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ec9cd-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ec9cd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec9cd-122">Request headers</span></span>
| <span data-ttu-id="ec9cd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec9cd-123">Header</span></span>       | <span data-ttu-id="ec9cd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ec9cd-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec9cd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec9cd-125">Authorization</span></span>  | <span data-ttu-id="ec9cd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec9cd-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec9cd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec9cd-128">Request body</span></span>
<span data-ttu-id="ec9cd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec9cd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec9cd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec9cd-130">Response</span></span>

<span data-ttu-id="ec9cd-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec9cd-131">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec9cd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ec9cd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec9cd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec9cd-133">Request</span></span>
<span data-ttu-id="ec9cd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec9cd-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec9cd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec9cd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="ec9cd-136">C#</span><span class="sxs-lookup"><span data-stu-id="ec9cd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec9cd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec9cd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec9cd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec9cd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec9cd-139">Java</span><span class="sxs-lookup"><span data-stu-id="ec9cd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ec9cd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec9cd-140">Response</span></span>
<span data-ttu-id="ec9cd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec9cd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->