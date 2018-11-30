---
title: Список участников
description: Получение списка участников объектов в вызове.
ms.openlocfilehash: a18dc609204712f1b7c7b31150975543277ffa67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076630"
---
# <a name="list-participants"></a><span data-ttu-id="71190-103">Список участников</span><span class="sxs-lookup"><span data-stu-id="71190-103">List participants</span></span>

> <span data-ttu-id="71190-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71190-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71190-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71190-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71190-106">Получение списка участников объектов в вызове.</span><span class="sxs-lookup"><span data-stu-id="71190-106">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="71190-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71190-107">Permissions</span></span>
<span data-ttu-id="71190-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71190-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71190-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71190-110">Permission type</span></span> | <span data-ttu-id="71190-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71190-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="71190-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71190-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="71190-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="71190-113">Not Supported</span></span>        |
| <span data-ttu-id="71190-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71190-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71190-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="71190-115">Not Supported</span></span>        |
| <span data-ttu-id="71190-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="71190-116">Application</span></span>     | <span data-ttu-id="71190-117">Нет</span><span class="sxs-lookup"><span data-stu-id="71190-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="71190-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71190-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71190-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71190-119">Optional query parameters</span></span>
<span data-ttu-id="71190-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="71190-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71190-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71190-121">Request headers</span></span>
| <span data-ttu-id="71190-122">Имя</span><span class="sxs-lookup"><span data-stu-id="71190-122">Name</span></span>          | <span data-ttu-id="71190-123">Описание</span><span class="sxs-lookup"><span data-stu-id="71190-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="71190-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71190-124">Authorization</span></span> | <span data-ttu-id="71190-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71190-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71190-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71190-127">Request body</span></span>
<span data-ttu-id="71190-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71190-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71190-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="71190-129">Response</span></span>
<span data-ttu-id="71190-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [участника](../resources/participant.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71190-130">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71190-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="71190-131">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="71190-132">Пример 1</span><span class="sxs-lookup"><span data-stu-id="71190-132">Example 1</span></span>

##### <a name="request"></a><span data-ttu-id="71190-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="71190-133">Request</span></span>
<span data-ttu-id="71190-134">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71190-134">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_participants"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants
```

##### <a name="response"></a><span data-ttu-id="71190-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="71190-135">Response</span></span>

> <span data-ttu-id="71190-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71190-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
Content-Length: 1152

{
  "value": [
    {
      "id": "id-value",
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
      "isInLobby": false,
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
      "metadata": "metadata-value"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="71190-138">Пример 2</span><span class="sxs-lookup"><span data-stu-id="71190-138">Example 2</span></span>

##### <a name="request"></a><span data-ttu-id="71190-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="71190-139">Request</span></span>

```http
GET /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

##### <a name="response"></a><span data-ttu-id="71190-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="71190-140">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
}-->
```json
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
<!-- {
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
