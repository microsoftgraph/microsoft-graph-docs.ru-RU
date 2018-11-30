---
title: Обновление объекта conversationThread
description: Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.
ms.openlocfilehash: 7fe8ded506246125d9e61f9c9d84c990a9838dbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026787"
---
# <a name="update-conversationthread"></a><span data-ttu-id="ea8cc-103">Обновление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="ea8cc-103">Update conversationthread</span></span>

<span data-ttu-id="ea8cc-104">Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-104">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea8cc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea8cc-105">Permissions</span></span>
<span data-ttu-id="ea8cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea8cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea8cc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea8cc-108">Permission type</span></span>      | <span data-ttu-id="ea8cc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea8cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea8cc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea8cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea8cc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea8cc-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea8cc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea8cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea8cc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-113">Not supported.</span></span>    |
|<span data-ttu-id="ea8cc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea8cc-114">Application</span></span> | <span data-ttu-id="ea8cc-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea8cc-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea8cc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea8cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ea8cc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea8cc-117">Request headers</span></span>
| <span data-ttu-id="ea8cc-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea8cc-118">Header</span></span>       | <span data-ttu-id="ea8cc-119">Значение</span><span class="sxs-lookup"><span data-stu-id="ea8cc-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea8cc-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea8cc-120">Authorization</span></span>  | <span data-ttu-id="ea8cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ea8cc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea8cc-123">Content-Type</span></span>  | <span data-ttu-id="ea8cc-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea8cc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea8cc-126">Request body</span></span>
<span data-ttu-id="ea8cc-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ea8cc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea8cc-130">Property</span></span>     | <span data-ttu-id="ea8cc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ea8cc-131">Type</span></span>   |<span data-ttu-id="ea8cc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea8cc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea8cc-133">isLocked</span><span class="sxs-lookup"><span data-stu-id="ea8cc-133">isLocked</span></span>|<span data-ttu-id="ea8cc-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea8cc-134">Boolean</span></span>|<span data-ttu-id="ea8cc-p105">Указывает, заблокирована ли цепочка. Чтобы запретить добавление сообщений, задайте значение `true`.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="ea8cc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea8cc-137">Response</span></span>

<span data-ttu-id="ea8cc-138">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-138">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea8cc-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ea8cc-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea8cc-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea8cc-140">Request</span></span>
<span data-ttu-id="ea8cc-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="ea8cc-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea8cc-142">Response</span></span>
<span data-ttu-id="ea8cc-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ea8cc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ],
  "isLocked": true 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
