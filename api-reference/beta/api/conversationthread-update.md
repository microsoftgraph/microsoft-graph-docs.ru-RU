---
title: Обновление объекта conversationThread
description: Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9654dbb15fcda9ee3084f504b114570083e5d551
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002696"
---
# <a name="update-conversationthread"></a><span data-ttu-id="f5b8c-103">Обновление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="f5b8c-103">Update conversationthread</span></span>

<span data-ttu-id="f5b8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5b8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5b8c-105">Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.</span><span class="sxs-lookup"><span data-stu-id="f5b8c-105">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5b8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b8c-106">Permissions</span></span>
<span data-ttu-id="f5b8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5b8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5b8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b8c-109">Permission type</span></span>      | <span data-ttu-id="f5b8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5b8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5b8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5b8c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f5b8c-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b8c-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f5b8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5b8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5b8c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b8c-114">Not supported.</span></span>    |
|<span data-ttu-id="f5b8c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5b8c-115">Application</span></span> | <span data-ttu-id="f5b8c-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b8c-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5b8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5b8c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f5b8c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5b8c-118">Request headers</span></span>
| <span data-ttu-id="f5b8c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5b8c-119">Header</span></span>       | <span data-ttu-id="f5b8c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f5b8c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5b8c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5b8c-121">Authorization</span></span>  | <span data-ttu-id="f5b8c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5b8c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f5b8c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5b8c-124">Content-Type</span></span>  | <span data-ttu-id="f5b8c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5b8c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5b8c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5b8c-127">Request body</span></span>
<span data-ttu-id="f5b8c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f5b8c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f5b8c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5b8c-131">Property</span></span>     | <span data-ttu-id="f5b8c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f5b8c-132">Type</span></span>   |<span data-ttu-id="f5b8c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f5b8c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5b8c-134">isLocked</span><span class="sxs-lookup"><span data-stu-id="f5b8c-134">isLocked</span></span>|<span data-ttu-id="f5b8c-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="f5b8c-135">Boolean</span></span>|<span data-ttu-id="f5b8c-p105">Указывает, заблокирована ли цепочка. Чтобы запретить добавление сообщений, задайте значение `true`.</span><span class="sxs-lookup"><span data-stu-id="f5b8c-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="f5b8c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b8c-138">Response</span></span>

<span data-ttu-id="f5b8c-139">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f5b8c-139">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5b8c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f5b8c-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5b8c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5b8c-141">Request</span></span>
<span data-ttu-id="f5b8c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5b8c-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5b8c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5b8c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
# <a name="c"></a>[<span data-ttu-id="f5b8c-144">C#</span><span class="sxs-lookup"><span data-stu-id="f5b8c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5b8c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5b8c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5b8c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5b8c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f5b8c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b8c-147">Response</span></span>
<span data-ttu-id="f5b8c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5b8c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ],
  "isLocked": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


