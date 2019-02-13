---
title: Список участников
description: Получение списка участников объектов в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc38af4a6bee4a380a001310303d67efb2705dcf
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967349"
---
# <a name="list-participants"></a><span data-ttu-id="7a1ae-103">Список участников</span><span class="sxs-lookup"><span data-stu-id="7a1ae-103">List participants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a1ae-104">Получение списка участников объектов в вызове.</span><span class="sxs-lookup"><span data-stu-id="7a1ae-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a1ae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a1ae-105">Permissions</span></span>

<span data-ttu-id="7a1ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a1ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a1ae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a1ae-108">Permission type</span></span> | <span data-ttu-id="7a1ae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a1ae-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="7a1ae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a1ae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a1ae-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7a1ae-111">Not Supported</span></span>        |
| <span data-ttu-id="7a1ae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a1ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a1ae-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7a1ae-113">Not Supported</span></span>        |
| <span data-ttu-id="7a1ae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a1ae-114">Application</span></span>     | <span data-ttu-id="7a1ae-115">Нет</span><span class="sxs-lookup"><span data-stu-id="7a1ae-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="7a1ae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a1ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a1ae-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a1ae-117">Optional query parameters</span></span>

<span data-ttu-id="7a1ae-118">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="7a1ae-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a1ae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a1ae-119">Request headers</span></span>

| <span data-ttu-id="7a1ae-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7a1ae-120">Name</span></span>          | <span data-ttu-id="7a1ae-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7a1ae-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7a1ae-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a1ae-122">Authorization</span></span> | <span data-ttu-id="7a1ae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a1ae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a1ae-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a1ae-125">Request body</span></span>

<span data-ttu-id="7a1ae-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a1ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a1ae-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a1ae-127">Response</span></span>

<span data-ttu-id="7a1ae-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [участника](../resources/participant.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7a1ae-128">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a1ae-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="7a1ae-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a1ae-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a1ae-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```http
GET https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="7a1ae-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a1ae-131">Response</span></span>

> <span data-ttu-id="7a1ae-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a1ae-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "user" : {
            "displayName": "Test User",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "1",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ]
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "phone": {
            "displayName": "+12345678890",
            "id": "+12345678890"
          }
        }
      },
      "mediaStreams": [
        {
          "sourceId": "2",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "application" : {
            "displayName": "Test BOT",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "3",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-list-participants.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
