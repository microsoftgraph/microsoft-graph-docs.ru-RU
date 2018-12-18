---
title: Список вложений
description: Получение списка объектов вложений.
author: angelgolfer-ms
ms.openlocfilehash: 49467c8b7576dfda8f47587acc1dc8d83f6ce445
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363658"
---
# <a name="list-attachments"></a><span data-ttu-id="dd90f-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="dd90f-103">List attachments</span></span>

> <span data-ttu-id="dd90f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dd90f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd90f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd90f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd90f-106">Получение списка объектов вложений.</span><span class="sxs-lookup"><span data-stu-id="dd90f-106">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd90f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd90f-107">Permissions</span></span>
<span data-ttu-id="dd90f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd90f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd90f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd90f-110">Permission type</span></span>      | <span data-ttu-id="dd90f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd90f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd90f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd90f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dd90f-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dd90f-113">Mail.Read</span></span>    |
|<span data-ttu-id="dd90f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd90f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd90f-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dd90f-115">Mail.Read</span></span>    |
|<span data-ttu-id="dd90f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd90f-116">Application</span></span> | <span data-ttu-id="dd90f-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dd90f-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd90f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd90f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dd90f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd90f-119">Optional query parameters</span></span>
<span data-ttu-id="dd90f-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dd90f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd90f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd90f-121">Request headers</span></span>
| <span data-ttu-id="dd90f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="dd90f-122">Name</span></span>       | <span data-ttu-id="dd90f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="dd90f-123">Type</span></span> | <span data-ttu-id="dd90f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dd90f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dd90f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd90f-125">Authorization</span></span>  | <span data-ttu-id="dd90f-126">string</span><span class="sxs-lookup"><span data-stu-id="dd90f-126">string</span></span>  | <span data-ttu-id="dd90f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd90f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd90f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd90f-129">Request body</span></span>
<span data-ttu-id="dd90f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd90f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd90f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd90f-131">Response</span></span>

<span data-ttu-id="dd90f-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd90f-132">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd90f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="dd90f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd90f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd90f-134">Request</span></span>
<span data-ttu-id="dd90f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd90f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="dd90f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd90f-136">Response</span></span>
<span data-ttu-id="dd90f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dd90f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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