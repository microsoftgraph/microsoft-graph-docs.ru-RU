---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 50d41b94300eaf93c6d0cd595e64facc982cb461
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872109"
---
# <a name="list-attachments"></a><span data-ttu-id="1475e-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="1475e-103">List attachments</span></span>

> <span data-ttu-id="1475e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1475e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1475e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1475e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1475e-106">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="1475e-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="1475e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1475e-107">Permissions</span></span>
<span data-ttu-id="1475e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1475e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1475e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1475e-110">Permission type</span></span>      | <span data-ttu-id="1475e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1475e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1475e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1475e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1475e-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1475e-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1475e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1475e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1475e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1475e-115">Not supported.</span></span>    |
|<span data-ttu-id="1475e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1475e-116">Application</span></span> | <span data-ttu-id="1475e-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1475e-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1475e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1475e-118">HTTP request</span></span>
<span data-ttu-id="1475e-119"><!-- { "blockType": "ignored" } -->Вложения для [записи](../resources/post.md) в [поток](../resources/conversationthread.md) , относящегося к [беседе](../resources/conversation.md) группы.</span><span class="sxs-lookup"><span data-stu-id="1475e-119"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1475e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1475e-120">Optional query parameters</span></span>
<span data-ttu-id="1475e-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1475e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1475e-122">В частности, можно использовать $разверните параметр запроса для включения всех встроенных вложений post остальные свойства post.</span><span class="sxs-lookup"><span data-stu-id="1475e-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="1475e-123">Пример:</span><span class="sxs-lookup"><span data-stu-id="1475e-123">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="1475e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1475e-124">Request headers</span></span>
| <span data-ttu-id="1475e-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1475e-125">Header</span></span>       | <span data-ttu-id="1475e-126">Значение</span><span class="sxs-lookup"><span data-stu-id="1475e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1475e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1475e-127">Authorization</span></span>  | <span data-ttu-id="1475e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1475e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1475e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1475e-130">Request body</span></span>
<span data-ttu-id="1475e-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1475e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1475e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1475e-132">Response</span></span>

<span data-ttu-id="1475e-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1475e-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1475e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1475e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1475e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1475e-135">Request</span></span>
<span data-ttu-id="1475e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1475e-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="1475e-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="1475e-137">Response</span></span>
<span data-ttu-id="1475e-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1475e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
