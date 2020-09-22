---
title: Создание объекта Message
description: С помощью этого API можно создать экземпляр Message в mailfolder.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 368c9809f3812fe2ac99553f1f09a70037cf26ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027757"
---
# <a name="create-message"></a><span data-ttu-id="51505-103">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="51505-103">Create Message</span></span>

<span data-ttu-id="51505-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51505-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51505-105">С помощью этого API можно создать экземпляр Message в mailfolder.</span><span class="sxs-lookup"><span data-stu-id="51505-105">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="51505-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51505-106">Permissions</span></span>
<span data-ttu-id="51505-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51505-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51505-109">Permission type</span></span>      | <span data-ttu-id="51505-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51505-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51505-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51505-111">Delegated (work or school account)</span></span> | <span data-ttu-id="51505-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51505-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="51505-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51505-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51505-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51505-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="51505-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51505-115">Application</span></span> | <span data-ttu-id="51505-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51505-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="51505-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51505-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="51505-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51505-118">Request headers</span></span>
| <span data-ttu-id="51505-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51505-119">Header</span></span>       | <span data-ttu-id="51505-120">Значение</span><span class="sxs-lookup"><span data-stu-id="51505-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51505-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51505-121">Authorization</span></span>  | <span data-ttu-id="51505-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51505-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51505-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51505-124">Content-Type</span></span>  | <span data-ttu-id="51505-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51505-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51505-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51505-127">Request body</span></span>
<span data-ttu-id="51505-128">Предоставьте в тексте запроса описание объекта [Message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51505-128">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="51505-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="51505-129">Response</span></span>

<span data-ttu-id="51505-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51505-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51505-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51505-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51505-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="51505-132">Request</span></span>
<span data-ttu-id="51505-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51505-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51505-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="51505-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="51505-135">C#</span><span class="sxs-lookup"><span data-stu-id="51505-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51505-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51505-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="51505-137">Предоставьте в тексте запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51505-137">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="51505-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="51505-138">Response</span></span>
<span data-ttu-id="51505-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51505-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


