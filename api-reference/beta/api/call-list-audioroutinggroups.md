---
title: Список звуковых группы маршрутизации
description: Получение списка объектов **audioRoutingGroup** .
ms.openlocfilehash: d188d8478b8bf57f45f0fa15eed9973cafba7b2f
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156006"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="b9438-103">Список звуковых группы маршрутизации</span><span class="sxs-lookup"><span data-stu-id="b9438-103">List audio routing groups</span></span>

> <span data-ttu-id="b9438-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9438-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9438-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9438-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9438-106">Получение списка объектов **audioRoutingGroup** .</span><span class="sxs-lookup"><span data-stu-id="b9438-106">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9438-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9438-107">Permissions</span></span>
<span data-ttu-id="b9438-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9438-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9438-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9438-110">Permission type</span></span>                        | <span data-ttu-id="b9438-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9438-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9438-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9438-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9438-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9438-113">Not Supported.</span></span>                               |
| <span data-ttu-id="b9438-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9438-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9438-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9438-115">Not Supported.</span></span>                               |
| <span data-ttu-id="b9438-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b9438-116">Application</span></span>     | <span data-ttu-id="b9438-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="b9438-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9438-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9438-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9438-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9438-119">Optional query parameters</span></span>
<span data-ttu-id="b9438-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b9438-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9438-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9438-121">Request headers</span></span>
| <span data-ttu-id="b9438-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b9438-122">Name</span></span>          | <span data-ttu-id="b9438-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b9438-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b9438-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9438-124">Authorization</span></span> | <span data-ttu-id="b9438-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9438-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9438-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9438-127">Request body</span></span>
<span data-ttu-id="b9438-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9438-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9438-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9438-129">Response</span></span>
<span data-ttu-id="b9438-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [audioRoutingGroup](../resources/audioroutinggroup.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b9438-130">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9438-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b9438-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b9438-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9438-132">Request</span></span>
<span data-ttu-id="b9438-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9438-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a><span data-ttu-id="b9438-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9438-134">Response</span></span>

> <span data-ttu-id="b9438-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9438-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
