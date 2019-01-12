---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5000ed8f65c0dd982a341ceff5c125dada073290
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983501"
---
# <a name="list-attachments"></a><span data-ttu-id="34245-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="34245-103">List attachments</span></span>

<span data-ttu-id="34245-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="34245-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="34245-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34245-105">Permissions</span></span>
<span data-ttu-id="34245-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34245-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34245-108">Permission type</span></span>      | <span data-ttu-id="34245-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34245-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34245-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34245-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34245-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34245-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="34245-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34245-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34245-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34245-113">Not supported.</span></span>    |
|<span data-ttu-id="34245-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34245-114">Application</span></span> | <span data-ttu-id="34245-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34245-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34245-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34245-116">HTTP request</span></span>
<span data-ttu-id="34245-117"><!-- { "blockType": "ignored" } -->Вложения для [записи](../resources/post.md) в [поток](../resources/conversationthread.md) , относящегося к [беседе](../resources/conversation.md) группы.</span><span class="sxs-lookup"><span data-stu-id="34245-117"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="34245-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="34245-118">Optional query parameters</span></span>
<span data-ttu-id="34245-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="34245-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="34245-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34245-120">Request headers</span></span>
| <span data-ttu-id="34245-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34245-121">Header</span></span>       | <span data-ttu-id="34245-122">Значение</span><span class="sxs-lookup"><span data-stu-id="34245-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="34245-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34245-123">Authorization</span></span>  | <span data-ttu-id="34245-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34245-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34245-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34245-126">Request body</span></span>
<span data-ttu-id="34245-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34245-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34245-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="34245-128">Response</span></span>

<span data-ttu-id="34245-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34245-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34245-130">Пример</span><span class="sxs-lookup"><span data-stu-id="34245-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34245-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="34245-131">Request</span></span>
<span data-ttu-id="34245-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34245-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="34245-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="34245-133">Response</span></span>
<span data-ttu-id="34245-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="34245-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
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
