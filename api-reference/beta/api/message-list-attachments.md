---
title: Список вложений
description: Получение списка объектов attachment, вложенных в сообщение.
ms.openlocfilehash: b4fee6d42b743f894d874e018eff9ba4e6ea2ec1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079202"
---
# <a name="list-attachments"></a><span data-ttu-id="1f387-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="1f387-103">List attachments</span></span>

> <span data-ttu-id="1f387-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f387-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f387-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f387-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f387-106">Получение списка объектов [attachment](../resources/attachment.md), вложенных в сообщение.</span><span class="sxs-lookup"><span data-stu-id="1f387-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f387-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f387-107">Permissions</span></span>
<span data-ttu-id="1f387-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f387-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f387-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f387-110">Permission type</span></span>      | <span data-ttu-id="1f387-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f387-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f387-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f387-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1f387-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1f387-113">Mail.Read</span></span>    |
|<span data-ttu-id="1f387-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f387-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f387-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1f387-115">Mail.Read</span></span>    |
|<span data-ttu-id="1f387-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f387-116">Application</span></span> | <span data-ttu-id="1f387-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1f387-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f387-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f387-118">HTTP request</span></span>
<span data-ttu-id="1f387-119"><!-- { "blockType": "ignored" } -->Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f387-119"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="1f387-120">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f387-120">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="1f387-p103">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="1f387-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f387-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f387-123">Optional query parameters</span></span>
<span data-ttu-id="1f387-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1f387-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1f387-125">В частности, можно использовать $разверните параметр запроса для включения всех встроенного вложений сообщений с помощью rest свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="1f387-125">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="1f387-126">Пример:</span><span class="sxs-lookup"><span data-stu-id="1f387-126">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="1f387-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f387-127">Request headers</span></span>
| <span data-ttu-id="1f387-128">Имя</span><span class="sxs-lookup"><span data-stu-id="1f387-128">Name</span></span>       | <span data-ttu-id="1f387-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1f387-129">Type</span></span> | <span data-ttu-id="1f387-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1f387-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1f387-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f387-131">Authorization</span></span>  | <span data-ttu-id="1f387-132">string</span><span class="sxs-lookup"><span data-stu-id="1f387-132">string</span></span>  | <span data-ttu-id="1f387-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f387-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f387-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f387-135">Request body</span></span>
<span data-ttu-id="1f387-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f387-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f387-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f387-137">Response</span></span>

<span data-ttu-id="1f387-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f387-138">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f387-139">Пример</span><span class="sxs-lookup"><span data-stu-id="1f387-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f387-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f387-140">Request</span></span>
<span data-ttu-id="1f387-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f387-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="1f387-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f387-142">Response</span></span>
<span data-ttu-id="1f387-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1f387-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->