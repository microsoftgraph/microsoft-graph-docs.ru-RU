---
title: Создание объекта Message
description: С помощью этого API можно создать экземпляр Message в mailfolder.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cf6d3bb3cc96d27c634295863555274037d11427
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979208"
---
# <a name="create-message"></a><span data-ttu-id="04155-103">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="04155-103">Create Message</span></span>

<span data-ttu-id="04155-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04155-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04155-105">С помощью этого API можно создать экземпляр Message в mailfolder.</span><span class="sxs-lookup"><span data-stu-id="04155-105">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="04155-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04155-106">Permissions</span></span>
<span data-ttu-id="04155-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04155-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04155-109">Permission type</span></span>      | <span data-ttu-id="04155-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04155-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04155-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04155-111">Delegated (work or school account)</span></span> | <span data-ttu-id="04155-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04155-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="04155-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04155-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04155-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04155-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="04155-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04155-115">Application</span></span> | <span data-ttu-id="04155-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04155-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="04155-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04155-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="04155-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04155-118">Request headers</span></span>
| <span data-ttu-id="04155-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04155-119">Header</span></span>       | <span data-ttu-id="04155-120">Значение</span><span class="sxs-lookup"><span data-stu-id="04155-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04155-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04155-121">Authorization</span></span>  | <span data-ttu-id="04155-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04155-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04155-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04155-124">Content-Type</span></span>  | <span data-ttu-id="04155-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04155-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04155-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04155-127">Request body</span></span>
<span data-ttu-id="04155-128">Предоставьте в тексте запроса описание объекта [Message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04155-128">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="04155-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="04155-129">Response</span></span>

<span data-ttu-id="04155-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04155-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04155-131">Пример</span><span class="sxs-lookup"><span data-stu-id="04155-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04155-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="04155-132">Request</span></span>
<span data-ttu-id="04155-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04155-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04155-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="04155-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/messages
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
# <a name="c"></a>[<span data-ttu-id="04155-135">C#</span><span class="sxs-lookup"><span data-stu-id="04155-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04155-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04155-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04155-137">Java</span><span class="sxs-lookup"><span data-stu-id="04155-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="04155-138">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04155-138">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="04155-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="04155-139">Response</span></span>
<span data-ttu-id="04155-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04155-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


