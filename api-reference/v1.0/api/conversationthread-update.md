---
title: Обновление объекта conversationThread
description: Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.
localization_priority: Normal
ms.openlocfilehash: a7f0738314bc071d5d084903fdc46b7fac1cf8cd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846496"
---
# <a name="update-conversationthread"></a><span data-ttu-id="95d67-103">Обновление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="95d67-103">Update conversationthread</span></span>

<span data-ttu-id="95d67-104">Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.</span><span class="sxs-lookup"><span data-stu-id="95d67-104">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="95d67-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95d67-105">Permissions</span></span>
<span data-ttu-id="95d67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95d67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95d67-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95d67-108">Permission type</span></span>      | <span data-ttu-id="95d67-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95d67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95d67-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95d67-110">Delegated (work or school account)</span></span> | <span data-ttu-id="95d67-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d67-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="95d67-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95d67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95d67-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95d67-113">Not supported.</span></span>    |
|<span data-ttu-id="95d67-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95d67-114">Application</span></span> | <span data-ttu-id="95d67-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d67-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95d67-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95d67-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="95d67-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95d67-117">Request headers</span></span>
| <span data-ttu-id="95d67-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95d67-118">Header</span></span>       | <span data-ttu-id="95d67-119">Значение</span><span class="sxs-lookup"><span data-stu-id="95d67-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95d67-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95d67-120">Authorization</span></span>  | <span data-ttu-id="95d67-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95d67-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95d67-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95d67-123">Content-Type</span></span>  | <span data-ttu-id="95d67-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95d67-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95d67-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95d67-126">Request body</span></span>
<span data-ttu-id="95d67-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="95d67-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="95d67-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="95d67-130">Property</span></span>     | <span data-ttu-id="95d67-131">Тип</span><span class="sxs-lookup"><span data-stu-id="95d67-131">Type</span></span>   |<span data-ttu-id="95d67-132">Описание</span><span class="sxs-lookup"><span data-stu-id="95d67-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95d67-133">isLocked</span><span class="sxs-lookup"><span data-stu-id="95d67-133">isLocked</span></span>|<span data-ttu-id="95d67-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="95d67-134">Boolean</span></span>|<span data-ttu-id="95d67-p105">Указывает, заблокирована ли цепочка. Чтобы запретить добавление сообщений, задайте значение `true`.</span><span class="sxs-lookup"><span data-stu-id="95d67-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="95d67-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="95d67-137">Response</span></span>

<span data-ttu-id="95d67-138">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95d67-138">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95d67-139">Пример</span><span class="sxs-lookup"><span data-stu-id="95d67-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95d67-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="95d67-140">Request</span></span>
<span data-ttu-id="95d67-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95d67-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="95d67-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="95d67-142">Response</span></span>
<span data-ttu-id="95d67-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="95d67-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
