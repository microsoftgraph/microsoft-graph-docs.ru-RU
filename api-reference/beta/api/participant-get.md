---
title: Получение участников
description: Извлечение свойств и связи объекта **участника** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c43c4b9bc1fca7652b1e44657fc03ab8ce6b6214
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945547"
---
# <a name="get-participant"></a><span data-ttu-id="91411-103">Получение участников</span><span class="sxs-lookup"><span data-stu-id="91411-103">Get participant</span></span>

> <span data-ttu-id="91411-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91411-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91411-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91411-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91411-106">Извлечение свойств и связи объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="91411-106">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91411-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91411-107">Permissions</span></span>
<span data-ttu-id="91411-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91411-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91411-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91411-110">Permission type</span></span> | <span data-ttu-id="91411-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91411-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="91411-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91411-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="91411-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="91411-113">Not Supported</span></span>        |
| <span data-ttu-id="91411-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91411-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91411-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="91411-115">Not Supported</span></span>        |
| <span data-ttu-id="91411-116">Application</span><span class="sxs-lookup"><span data-stu-id="91411-116">Application</span></span>     | <span data-ttu-id="91411-117">Нет</span><span class="sxs-lookup"><span data-stu-id="91411-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="91411-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91411-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91411-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91411-119">Optional query parameters</span></span>
<span data-ttu-id="91411-120">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="91411-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91411-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91411-121">Request headers</span></span>
| <span data-ttu-id="91411-122">Имя</span><span class="sxs-lookup"><span data-stu-id="91411-122">Name</span></span>          | <span data-ttu-id="91411-123">Описание</span><span class="sxs-lookup"><span data-stu-id="91411-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="91411-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91411-124">Authorization</span></span> | <span data-ttu-id="91411-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91411-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91411-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91411-127">Request body</span></span>
<span data-ttu-id="91411-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91411-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91411-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="91411-129">Response</span></span>
<span data-ttu-id="91411-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [участника](../resources/participant.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="91411-130">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91411-131">Пример</span><span class="sxs-lookup"><span data-stu-id="91411-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="91411-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="91411-132">Request</span></span>
<span data-ttu-id="91411-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91411-133">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="91411-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="91411-134">Response</span></span>

> <span data-ttu-id="91411-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91411-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
