---
title: Список вложений
description: Получение списка объектов вложений.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a54e5ecc6b3880d923be62cfd0895a9262ec7e89
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042396"
---
# <a name="list-attachments"></a><span data-ttu-id="ed644-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="ed644-103">List attachments</span></span>

<span data-ttu-id="ed644-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed644-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed644-105">Получение списка объектов вложений.</span><span class="sxs-lookup"><span data-stu-id="ed644-105">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ed644-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed644-106">Permissions</span></span>
<span data-ttu-id="ed644-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed644-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed644-109">Permission type</span></span>      | <span data-ttu-id="ed644-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed644-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed644-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed644-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed644-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ed644-112">Mail.Read</span></span>    |
|<span data-ttu-id="ed644-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed644-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed644-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ed644-114">Mail.Read</span></span>    |
|<span data-ttu-id="ed644-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed644-115">Application</span></span> | <span data-ttu-id="ed644-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ed644-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed644-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed644-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed644-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ed644-118">Optional query parameters</span></span>
<span data-ttu-id="ed644-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ed644-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed644-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed644-120">Request headers</span></span>
| <span data-ttu-id="ed644-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ed644-121">Name</span></span>       | <span data-ttu-id="ed644-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ed644-122">Type</span></span> | <span data-ttu-id="ed644-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ed644-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ed644-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed644-124">Authorization</span></span>  | <span data-ttu-id="ed644-125">string</span><span class="sxs-lookup"><span data-stu-id="ed644-125">string</span></span>  | <span data-ttu-id="ed644-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed644-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed644-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed644-128">Request body</span></span>
<span data-ttu-id="ed644-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed644-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed644-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed644-130">Response</span></span>

<span data-ttu-id="ed644-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed644-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed644-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ed644-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed644-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed644-133">Request</span></span>
<span data-ttu-id="ed644-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed644-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed644-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed644-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "eventmessage_get_attachments_beta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="ed644-136">C#</span><span class="sxs-lookup"><span data-stu-id="ed644-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/eventmessage-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed644-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed644-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/eventmessage-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed644-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed644-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/eventmessage-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed644-139">Java</span><span class="sxs-lookup"><span data-stu-id="ed644-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/eventmessage-get-attachments-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ed644-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed644-140">Response</span></span>
<span data-ttu-id="ed644-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed644-141">Here is an example of the response.</span></span> <span data-ttu-id="ed644-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ed644-142">Note: The response object shown here might be shortened for readability.</span></span>
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
