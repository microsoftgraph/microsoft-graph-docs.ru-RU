---
title: Получение Чатмессажехостедимаже
description: Получение размещенного изображения в chatMessage.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7a8bf0fe79df064c7d53b987e1b9aa5ccddbc1cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943599"
---
# <a name="get-chatmessagehostedimage"></a><span data-ttu-id="6249f-103">Получение Чатмессажехостедимаже</span><span class="sxs-lookup"><span data-stu-id="6249f-103">Get chatMessageHostedImage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6249f-104">Получение [размещенного изображения](../resources/chatmessagehostedimage.md) в [chatMessage](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="6249f-104">Retrieve a [hosted image](../resources/chatmessagehostedimage.md) in a [chatMessage](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6249f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6249f-105">Permissions</span></span>

<span data-ttu-id="6249f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6249f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6249f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6249f-108">Permission Type</span></span>|<span data-ttu-id="6249f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6249f-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="6249f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6249f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6249f-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6249f-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="6249f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6249f-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6249f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6249f-113">Not supported.</span></span>|
|<span data-ttu-id="6249f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6249f-114">Application</span></span>| <span data-ttu-id="6249f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6249f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6249f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6249f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages/{id}
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages/{id}
GET /chats/{id}/messages/{id}/hostedImages/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6249f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6249f-117">Optional query parameters</span></span>

<span data-ttu-id="6249f-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6249f-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6249f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6249f-119">Request headers</span></span>

| <span data-ttu-id="6249f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6249f-120">Header</span></span>       | <span data-ttu-id="6249f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6249f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6249f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6249f-122">Authorization</span></span>  | <span data-ttu-id="6249f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6249f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6249f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6249f-125">Request body</span></span>

<span data-ttu-id="6249f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6249f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6249f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6249f-127">Response</span></span>

<span data-ttu-id="6249f-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и размещенный объект [Image](../resources/chatmessagehostedimage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6249f-128">If successful, this method returns a `200 OK` response code and a [hosted image](../resources/chatmessagehostedimage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6249f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6249f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6249f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6249f-130">Request</span></span>

<span data-ttu-id="6249f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6249f-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6249f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6249f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6249f-133">C#</span><span class="sxs-lookup"><span data-stu-id="6249f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6249f-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="6249f-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6249f-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6249f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6249f-136">Java</span><span class="sxs-lookup"><span data-stu-id="6249f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6249f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6249f-137">Response</span></span>

<span data-ttu-id="6249f-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6249f-138">Here is an example of the response.</span></span> 

><span data-ttu-id="6249f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6249f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "url": "url-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat message image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
