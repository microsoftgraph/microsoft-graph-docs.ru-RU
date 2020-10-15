---
title: Список вложений
description: Получение списка объектов вложений.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 99ab137ac28fb03f99db7b47474572e3e5ba3609
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459741"
---
# <a name="list-attachments"></a><span data-ttu-id="13007-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="13007-103">List attachments</span></span>

<span data-ttu-id="13007-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13007-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13007-105">Получение списка объектов вложений.</span><span class="sxs-lookup"><span data-stu-id="13007-105">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="13007-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13007-106">Permissions</span></span>
<span data-ttu-id="13007-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13007-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13007-109">Permission type</span></span>      | <span data-ttu-id="13007-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13007-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13007-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13007-111">Delegated (work or school account)</span></span> | <span data-ttu-id="13007-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13007-112">Mail.Read</span></span>    |
|<span data-ttu-id="13007-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13007-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13007-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13007-114">Mail.Read</span></span>    |
|<span data-ttu-id="13007-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13007-115">Application</span></span> | <span data-ttu-id="13007-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="13007-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="13007-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13007-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="13007-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="13007-118">Optional query parameters</span></span>
<span data-ttu-id="13007-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="13007-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13007-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13007-120">Request headers</span></span>
| <span data-ttu-id="13007-121">Имя</span><span class="sxs-lookup"><span data-stu-id="13007-121">Name</span></span>       | <span data-ttu-id="13007-122">Тип</span><span class="sxs-lookup"><span data-stu-id="13007-122">Type</span></span> | <span data-ttu-id="13007-123">Описание</span><span class="sxs-lookup"><span data-stu-id="13007-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="13007-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="13007-124">Authorization</span></span>  | <span data-ttu-id="13007-125">string</span><span class="sxs-lookup"><span data-stu-id="13007-125">string</span></span>  | <span data-ttu-id="13007-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13007-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13007-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13007-128">Request body</span></span>
<span data-ttu-id="13007-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13007-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13007-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="13007-130">Response</span></span>

<span data-ttu-id="13007-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13007-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13007-132">Пример</span><span class="sxs-lookup"><span data-stu-id="13007-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13007-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="13007-133">Request</span></span>
<span data-ttu-id="13007-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13007-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13007-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="13007-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "eventmessage_get_attachments_v1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="13007-136">C#</span><span class="sxs-lookup"><span data-stu-id="13007-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/eventmessage-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13007-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13007-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/eventmessage-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13007-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13007-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/eventmessage-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13007-139">Java</span><span class="sxs-lookup"><span data-stu-id="13007-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/eventmessage-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13007-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="13007-140">Response</span></span>
<span data-ttu-id="13007-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13007-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "eventmessage_get_attachments_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
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
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
