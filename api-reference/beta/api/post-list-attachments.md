---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 893ae044c1b201b104fe96738c10e639307deb9c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332119"
---
# <a name="list-attachments"></a><span data-ttu-id="f9d06-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="f9d06-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9d06-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="f9d06-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9d06-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9d06-105">Permissions</span></span>
<span data-ttu-id="f9d06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9d06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9d06-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9d06-108">Permission type</span></span>      | <span data-ttu-id="f9d06-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9d06-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9d06-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9d06-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9d06-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9d06-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9d06-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9d06-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9d06-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9d06-113">Not supported.</span></span>    |
|<span data-ttu-id="f9d06-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9d06-114">Application</span></span> | <span data-ttu-id="f9d06-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9d06-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9d06-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9d06-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f9d06-117">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="f9d06-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9d06-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9d06-118">Optional query parameters</span></span>
<span data-ttu-id="f9d06-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9d06-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f9d06-120">В частности, вы можете использовать параметр запроса $expand, чтобы включить все вложенные вложения со всеми остальными свойствами POST.</span><span class="sxs-lookup"><span data-stu-id="f9d06-120">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="f9d06-121">Пример:</span><span class="sxs-lookup"><span data-stu-id="f9d06-121">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="f9d06-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9d06-122">Request headers</span></span>
| <span data-ttu-id="f9d06-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9d06-123">Header</span></span>       | <span data-ttu-id="f9d06-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f9d06-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9d06-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9d06-125">Authorization</span></span>  | <span data-ttu-id="f9d06-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9d06-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9d06-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9d06-128">Request body</span></span>
<span data-ttu-id="f9d06-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9d06-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9d06-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9d06-130">Response</span></span>

<span data-ttu-id="f9d06-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9d06-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9d06-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f9d06-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9d06-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9d06-133">Request</span></span>
<span data-ttu-id="f9d06-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9d06-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="f9d06-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9d06-135">Response</span></span>
<span data-ttu-id="f9d06-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9d06-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
