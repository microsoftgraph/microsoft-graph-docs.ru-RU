---
title: Обновление объекта conversationThread
description: Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 2127b85b048a3c62baeabfae34eaa3806979cee8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455291"
---
# <a name="update-conversationthread"></a><span data-ttu-id="1ab78-103">Обновление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="1ab78-103">Update conversationthread</span></span>

<span data-ttu-id="1ab78-104">Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.</span><span class="sxs-lookup"><span data-stu-id="1ab78-104">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ab78-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ab78-105">Permissions</span></span>
<span data-ttu-id="1ab78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ab78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ab78-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ab78-108">Permission type</span></span>      | <span data-ttu-id="1ab78-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ab78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ab78-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ab78-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ab78-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ab78-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ab78-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ab78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ab78-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ab78-113">Not supported.</span></span>    |
|<span data-ttu-id="1ab78-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ab78-114">Application</span></span> | <span data-ttu-id="1ab78-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ab78-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ab78-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ab78-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1ab78-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ab78-117">Request headers</span></span>
| <span data-ttu-id="1ab78-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ab78-118">Header</span></span>       | <span data-ttu-id="1ab78-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1ab78-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ab78-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ab78-120">Authorization</span></span>  | <span data-ttu-id="1ab78-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ab78-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1ab78-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ab78-123">Content-Type</span></span>  | <span data-ttu-id="1ab78-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ab78-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ab78-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ab78-126">Request body</span></span>
<span data-ttu-id="1ab78-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1ab78-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1ab78-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ab78-130">Property</span></span>     | <span data-ttu-id="1ab78-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1ab78-131">Type</span></span>   |<span data-ttu-id="1ab78-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1ab78-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ab78-133">isLocked</span><span class="sxs-lookup"><span data-stu-id="1ab78-133">isLocked</span></span>|<span data-ttu-id="1ab78-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="1ab78-134">Boolean</span></span>|<span data-ttu-id="1ab78-p105">Указывает, заблокирована ли цепочка. Чтобы запретить добавление сообщений, задайте значение `true`.</span><span class="sxs-lookup"><span data-stu-id="1ab78-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="1ab78-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ab78-137">Response</span></span>

<span data-ttu-id="1ab78-138">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ab78-138">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ab78-139">Пример</span><span class="sxs-lookup"><span data-stu-id="1ab78-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ab78-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ab78-140">Request</span></span>
<span data-ttu-id="1ab78-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ab78-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1ab78-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ab78-142">Response</span></span>
<span data-ttu-id="1ab78-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ab78-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
