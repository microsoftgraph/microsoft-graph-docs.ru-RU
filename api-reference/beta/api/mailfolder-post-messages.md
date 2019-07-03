---
title: Создание объекта Message
description: С помощью этого API можно создать экземпляр Message в mailfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d576854517c9fb4cf2d34fa7cf33d2388b452b95
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449682"
---
# <a name="create-message"></a><span data-ttu-id="a0072-103">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="a0072-103">Create Message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0072-104">С помощью этого API можно создать экземпляр Message в mailfolder.</span><span class="sxs-lookup"><span data-stu-id="a0072-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0072-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0072-105">Permissions</span></span>
<span data-ttu-id="a0072-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0072-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0072-108">Permission type</span></span>      | <span data-ttu-id="a0072-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0072-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0072-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0072-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0072-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0072-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a0072-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0072-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0072-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0072-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a0072-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0072-114">Application</span></span> | <span data-ttu-id="a0072-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0072-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0072-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0072-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="a0072-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0072-117">Request headers</span></span>
| <span data-ttu-id="a0072-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0072-118">Header</span></span>       | <span data-ttu-id="a0072-119">Значение</span><span class="sxs-lookup"><span data-stu-id="a0072-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0072-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0072-120">Authorization</span></span>  | <span data-ttu-id="a0072-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0072-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a0072-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0072-123">Content-Type</span></span>  | <span data-ttu-id="a0072-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0072-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0072-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0072-126">Request body</span></span>
<span data-ttu-id="a0072-127">Предоставьте в тексте запроса описание объекта [Message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0072-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0072-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0072-128">Response</span></span>

<span data-ttu-id="a0072-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0072-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0072-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a0072-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0072-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0072-131">Request</span></span>
<span data-ttu-id="a0072-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0072-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a0072-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0072-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a0072-134">C#</span><span class="sxs-lookup"><span data-stu-id="a0072-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0072-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="a0072-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a0072-136">Предоставьте в тексте запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0072-136">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a0072-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0072-137">Response</span></span>
<span data-ttu-id="a0072-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0072-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
