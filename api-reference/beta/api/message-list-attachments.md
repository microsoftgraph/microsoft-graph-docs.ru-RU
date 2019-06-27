---
title: Список вложений
description: Получение списка объектов attachment, вложенных в сообщение.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 649cc2a58c5a103e584cf8388ba8713ef6bcec15
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266068"
---
# <a name="list-attachments"></a><span data-ttu-id="91e46-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="91e46-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91e46-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в сообщение.</span><span class="sxs-lookup"><span data-stu-id="91e46-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="91e46-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91e46-105">Permissions</span></span>
<span data-ttu-id="91e46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91e46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91e46-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91e46-108">Permission type</span></span>      | <span data-ttu-id="91e46-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91e46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91e46-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91e46-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91e46-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="91e46-111">Mail.Read</span></span>    |
|<span data-ttu-id="91e46-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91e46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91e46-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="91e46-113">Mail.Read</span></span>    |
|<span data-ttu-id="91e46-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91e46-114">Application</span></span> | <span data-ttu-id="91e46-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="91e46-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="91e46-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91e46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="91e46-117">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="91e46-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="91e46-118">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="91e46-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="91e46-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="91e46-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91e46-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91e46-121">Optional query parameters</span></span>
<span data-ttu-id="91e46-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91e46-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="91e46-123">В частности, параметр запроса $expand можно использовать для включения всех вложений в сообщения, встроенных в остальные свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="91e46-123">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="91e46-124">Пример:</span><span class="sxs-lookup"><span data-stu-id="91e46-124">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="91e46-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91e46-125">Request headers</span></span>
| <span data-ttu-id="91e46-126">Имя</span><span class="sxs-lookup"><span data-stu-id="91e46-126">Name</span></span>       | <span data-ttu-id="91e46-127">Тип</span><span class="sxs-lookup"><span data-stu-id="91e46-127">Type</span></span> | <span data-ttu-id="91e46-128">Описание</span><span class="sxs-lookup"><span data-stu-id="91e46-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="91e46-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="91e46-129">Authorization</span></span>  | <span data-ttu-id="91e46-130">string</span><span class="sxs-lookup"><span data-stu-id="91e46-130">string</span></span>  | <span data-ttu-id="91e46-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91e46-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91e46-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91e46-133">Request body</span></span>
<span data-ttu-id="91e46-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91e46-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91e46-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="91e46-135">Response</span></span>

<span data-ttu-id="91e46-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91e46-136">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91e46-137">Пример</span><span class="sxs-lookup"><span data-stu-id="91e46-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91e46-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="91e46-138">Request</span></span>
<span data-ttu-id="91e46-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91e46-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="91e46-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="91e46-140">Response</span></span>
<span data-ttu-id="91e46-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91e46-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="91e46-144">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="91e46-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="91e46-145">C#</span><span class="sxs-lookup"><span data-stu-id="91e46-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91e46-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="91e46-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="91e46-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="91e46-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_attachments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-list-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
