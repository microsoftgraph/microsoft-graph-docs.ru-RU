---
title: Список вложений
description: Получение списка объектов вложений.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d5a8994023c078b646f1bd7f0465acc247932ee7
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457743"
---
# <a name="list-attachments"></a><span data-ttu-id="1c795-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="1c795-103">List attachments</span></span>

<span data-ttu-id="1c795-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c795-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c795-105">Получение списка объектов вложений.</span><span class="sxs-lookup"><span data-stu-id="1c795-105">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c795-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c795-106">Permissions</span></span>
<span data-ttu-id="1c795-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c795-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c795-109">Permission type</span></span>      | <span data-ttu-id="1c795-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c795-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c795-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c795-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c795-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1c795-112">Mail.Read</span></span>    |
|<span data-ttu-id="1c795-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c795-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c795-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1c795-114">Mail.Read</span></span>    |
|<span data-ttu-id="1c795-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c795-115">Application</span></span> | <span data-ttu-id="1c795-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1c795-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c795-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c795-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c795-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1c795-118">Optional query parameters</span></span>
<span data-ttu-id="1c795-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1c795-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c795-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c795-120">Request headers</span></span>
| <span data-ttu-id="1c795-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1c795-121">Name</span></span>       | <span data-ttu-id="1c795-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1c795-122">Type</span></span> | <span data-ttu-id="1c795-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1c795-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c795-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c795-124">Authorization</span></span>  | <span data-ttu-id="1c795-125">string</span><span class="sxs-lookup"><span data-stu-id="1c795-125">string</span></span>  | <span data-ttu-id="1c795-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c795-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c795-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c795-128">Request body</span></span>
<span data-ttu-id="1c795-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c795-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c795-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c795-130">Response</span></span>

<span data-ttu-id="1c795-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c795-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c795-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1c795-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c795-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c795-133">Request</span></span>
<span data-ttu-id="1c795-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c795-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c795-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c795-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "eventmessage_get_attachments_beta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="1c795-136">C#</span><span class="sxs-lookup"><span data-stu-id="1c795-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/eventmessage-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c795-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c795-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/eventmessage-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c795-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c795-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/eventmessage-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c795-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c795-139">Response</span></span>
<span data-ttu-id="1c795-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c795-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "eventmessage_get_attachments_beta",
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
      "@odata.type":"#microsoft.graph.fileAttachment",
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
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
