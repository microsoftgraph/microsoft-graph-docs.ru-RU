---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
ms.openlocfilehash: b1a7ea8778b2ff25ad8e3159697d12aafe180506
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028373"
---
# <a name="list-attachments"></a><span data-ttu-id="9df5d-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="9df5d-103">List attachments</span></span>

<span data-ttu-id="9df5d-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="9df5d-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="9df5d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9df5d-105">Permissions</span></span>
<span data-ttu-id="9df5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9df5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9df5d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9df5d-108">Permission type</span></span>      | <span data-ttu-id="9df5d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9df5d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9df5d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9df5d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9df5d-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9df5d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9df5d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9df5d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9df5d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9df5d-113">Not supported.</span></span>    |
|<span data-ttu-id="9df5d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9df5d-114">Application</span></span> | <span data-ttu-id="9df5d-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9df5d-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9df5d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9df5d-116">HTTP request</span></span>
<span data-ttu-id="9df5d-117"><!-- { "blockType": "ignored" } -->Вложения для [записи](../resources/post.md) в [поток](../resources/conversationthread.md) , относящегося к [беседе](../resources/conversation.md) группы.</span><span class="sxs-lookup"><span data-stu-id="9df5d-117"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9df5d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9df5d-118">Optional query parameters</span></span>
<span data-ttu-id="9df5d-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9df5d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9df5d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9df5d-120">Request headers</span></span>
| <span data-ttu-id="9df5d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9df5d-121">Header</span></span>       | <span data-ttu-id="9df5d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9df5d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9df5d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9df5d-123">Authorization</span></span>  | <span data-ttu-id="9df5d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9df5d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9df5d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9df5d-126">Request body</span></span>
<span data-ttu-id="9df5d-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9df5d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9df5d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9df5d-128">Response</span></span>

<span data-ttu-id="9df5d-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9df5d-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9df5d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9df5d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9df5d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9df5d-131">Request</span></span>
<span data-ttu-id="9df5d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9df5d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="9df5d-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9df5d-133">Response</span></span>
<span data-ttu-id="9df5d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9df5d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
