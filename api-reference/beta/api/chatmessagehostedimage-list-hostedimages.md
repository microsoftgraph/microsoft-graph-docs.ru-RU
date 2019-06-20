---
title: Перечисление объектов chatMessageHostedImage в объекте chatmessage
description: Перечисление всех размещенных изображений в объекте chatMessage.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 2511afe199ecadf6d206037e2820708abe737ce8
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/20/2019
ms.locfileid: "35085842"
---
# <a name="list-chatmessagehostedimages-in-a-chatmessage"></a><span data-ttu-id="9721c-103">Перечисление объектов chatMessageHostedImage в объекте chatMessage</span><span class="sxs-lookup"><span data-stu-id="9721c-103">List chatMessageHostedImages in a chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9721c-104">Перечисление всех [размещенных изображений](../resources/chatmessagehostedimage.md) в объекте [chatMessage](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="9721c-104">List all [hosted images](../resources/chatmessagehostedimage.md) in a [chatMessage](../resources/chatmessage.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9721c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9721c-105">Permissions</span></span>

<span data-ttu-id="9721c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9721c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9721c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9721c-108">Permission Type</span></span>|<span data-ttu-id="9721c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9721c-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9721c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9721c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9721c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9721c-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="9721c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9721c-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9721c-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9721c-113">Not supported</span></span>|
|<span data-ttu-id="9721c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9721c-114">Application</span></span>| <span data-ttu-id="9721c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9721c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9721c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9721c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/hostedImages
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}/hostedImages
GET /chats/{id}/messages/{id}/hostedImages
GET /users/{id}/chats/{id}/messages/{id}/hostedImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9721c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9721c-117">Optional query parameters</span></span>

<span data-ttu-id="9721c-118">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9721c-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9721c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9721c-119">Request headers</span></span>

| <span data-ttu-id="9721c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9721c-120">Header</span></span>       | <span data-ttu-id="9721c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9721c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9721c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9721c-122">Authorization</span></span>  | <span data-ttu-id="9721c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9721c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9721c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9721c-125">Request body</span></span>

<span data-ttu-id="9721c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9721c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9721c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9721c-127">Response</span></span>

<span data-ttu-id="9721c-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [hostedImage](../resources/chatmessagehostedimage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9721c-128">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/chatmessagehostedimage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9721c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9721c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9721c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9721c-130">Request</span></span>

<span data-ttu-id="9721c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9721c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/hostedImages
```

##### <a name="response"></a><span data-ttu-id="9721c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9721c-132">Response</span></span>

<span data-ttu-id="9721c-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9721c-133">Here is an example of the response.</span></span> 

><span data-ttu-id="9721c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9721c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "value": [
    {
        "id": "id-value",
        "url": "url-value"
    },
    {
        "id": "id-value",
        "url": "url-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List hosted images in a chatmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedimage-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
