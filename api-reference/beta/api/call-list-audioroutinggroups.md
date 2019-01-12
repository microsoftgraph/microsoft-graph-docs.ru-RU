---
title: Список звуковых группы маршрутизации
description: Получение списка объектов **audioRoutingGroup** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2df2095e8d76332e94a32f802be3f36239cd8988
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976242"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="d78b0-103">Список звуковых группы маршрутизации</span><span class="sxs-lookup"><span data-stu-id="d78b0-103">List audio routing groups</span></span>

> <span data-ttu-id="d78b0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d78b0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d78b0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78b0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d78b0-106">Получение списка объектов **audioRoutingGroup** .</span><span class="sxs-lookup"><span data-stu-id="d78b0-106">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d78b0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d78b0-107">Permissions</span></span>
<span data-ttu-id="d78b0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d78b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d78b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d78b0-110">Permission type</span></span>                        | <span data-ttu-id="d78b0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d78b0-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d78b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d78b0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d78b0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78b0-113">Not Supported.</span></span>                               |
| <span data-ttu-id="d78b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d78b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d78b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78b0-115">Not Supported.</span></span>                               |
| <span data-ttu-id="d78b0-116">Application</span><span class="sxs-lookup"><span data-stu-id="d78b0-116">Application</span></span>     | <span data-ttu-id="d78b0-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="d78b0-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d78b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d78b0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d78b0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d78b0-119">Optional query parameters</span></span>
<span data-ttu-id="d78b0-120">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="d78b0-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d78b0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d78b0-121">Request headers</span></span>
| <span data-ttu-id="d78b0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d78b0-122">Name</span></span>          | <span data-ttu-id="d78b0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d78b0-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d78b0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d78b0-124">Authorization</span></span> | <span data-ttu-id="d78b0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d78b0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d78b0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d78b0-127">Request body</span></span>
<span data-ttu-id="d78b0-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d78b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d78b0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d78b0-129">Response</span></span>
<span data-ttu-id="d78b0-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [audioRoutingGroup](../resources/audioroutinggroup.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d78b0-130">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d78b0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d78b0-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d78b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d78b0-132">Request</span></span>
<span data-ttu-id="d78b0-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d78b0-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a><span data-ttu-id="d78b0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d78b0-134">Response</span></span>

> <span data-ttu-id="d78b0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d78b0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup",
  "isCollection": true 
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": [
    {
      "id": "oneToOne",
      "routingMode": "oneToOne",
      "sources": [
        "632899f8-2ea1-4604-8413-27bd2892079f"
      ],
      "receivers": [
        "550fae72-d251-43ec-868c-373732c2704f",
        "72f988bf-86f1-41af-91ab-2d7cd011db47"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List audioRoutingGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
