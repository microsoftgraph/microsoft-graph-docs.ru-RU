---
title: Получение участника
description: Получение свойств и связей объекта **участника** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fc60b6f6a4ed1a1b1e97c9bdfddec37384faf05d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265613"
---
# <a name="get-participant"></a><span data-ttu-id="62b16-103">Получение участника</span><span class="sxs-lookup"><span data-stu-id="62b16-103">Get participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62b16-104">Получение свойств и связей объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="62b16-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="62b16-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62b16-105">Permissions</span></span>
<span data-ttu-id="62b16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62b16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62b16-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62b16-108">Permission type</span></span> | <span data-ttu-id="62b16-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62b16-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="62b16-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62b16-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="62b16-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="62b16-111">Not Supported</span></span>        |
| <span data-ttu-id="62b16-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62b16-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62b16-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="62b16-113">Not Supported</span></span>        |
| <span data-ttu-id="62b16-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62b16-114">Application</span></span>     | <span data-ttu-id="62b16-115">Нет</span><span class="sxs-lookup"><span data-stu-id="62b16-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="62b16-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62b16-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62b16-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62b16-117">Optional query parameters</span></span>
<span data-ttu-id="62b16-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="62b16-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62b16-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62b16-119">Request headers</span></span>
| <span data-ttu-id="62b16-120">Имя</span><span class="sxs-lookup"><span data-stu-id="62b16-120">Name</span></span>          | <span data-ttu-id="62b16-121">Описание</span><span class="sxs-lookup"><span data-stu-id="62b16-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="62b16-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62b16-122">Authorization</span></span> | <span data-ttu-id="62b16-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62b16-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62b16-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62b16-125">Request body</span></span>
<span data-ttu-id="62b16-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62b16-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62b16-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="62b16-127">Response</span></span>
<span data-ttu-id="62b16-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [участника](../resources/participant.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="62b16-128">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62b16-129">Пример</span><span class="sxs-lookup"><span data-stu-id="62b16-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="62b16-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="62b16-130">Request</span></span>
<span data-ttu-id="62b16-131">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62b16-131">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="62b16-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="62b16-132">Response</span></span>

> <span data-ttu-id="62b16-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62b16-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "initiatedBy": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    },
    "status": "recordingCapable"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="62b16-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="62b16-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62b16-136">C#</span><span class="sxs-lookup"><span data-stu-id="62b16-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-participant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62b16-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="62b16-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-participant-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="62b16-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="62b16-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-participant-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/participant-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/participant-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
