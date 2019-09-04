---
title: Получение расписания
description: Получение свойств и связей объекта **расписания** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d7fc8145a17cd2a6609b1a203f12e4836cb030e2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724759"
---
# <a name="get-schedule"></a><span data-ttu-id="f49e2-103">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="f49e2-103">Get schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f49e2-104">Получение свойств и связей объекта [расписания](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="f49e2-104">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="f49e2-105">Процесс создания расписания соответствует [одной рекомендации API для долгосрочных операций, выполняемых на основе ресурсов (РЕЛО)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="f49e2-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="f49e2-106">Когда клиенты используют [метод PUT](team-put-schedule.md), если расписание подготовлено, операция обновляет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="f49e2-106">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="f49e2-107">Во время подготовки расписания клиенты могут использовать метод GET для получения расписания и просмотра `provisionStatus` свойства для текущего состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="f49e2-107">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="f49e2-108">Если не удалось выполнить подготовку, клиенты могут получить дополнительные сведения из `provisionStatusCode` свойства.</span><span class="sxs-lookup"><span data-stu-id="f49e2-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="f49e2-109">Клиенты также могут проверить конфигурацию расписания.</span><span class="sxs-lookup"><span data-stu-id="f49e2-109">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="f49e2-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f49e2-110">Permissions</span></span>

<span data-ttu-id="f49e2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f49e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f49e2-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f49e2-113">Permission type</span></span>      | <span data-ttu-id="f49e2-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f49e2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f49e2-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f49e2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f49e2-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f49e2-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f49e2-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f49e2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f49e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f49e2-118">Not supported.</span></span>    |
|<span data-ttu-id="f49e2-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f49e2-119">Application</span></span> | <span data-ttu-id="f49e2-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f49e2-120">Not supported.</span></span> |

> <span data-ttu-id="f49e2-121">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f49e2-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f49e2-122">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="f49e2-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f49e2-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f49e2-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="f49e2-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f49e2-124">Request headers</span></span>

| <span data-ttu-id="f49e2-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f49e2-125">Header</span></span>       | <span data-ttu-id="f49e2-126">Значение</span><span class="sxs-lookup"><span data-stu-id="f49e2-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f49e2-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f49e2-127">Authorization</span></span>  | <span data-ttu-id="f49e2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f49e2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f49e2-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f49e2-130">Content-Type</span></span>  | <span data-ttu-id="f49e2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f49e2-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f49e2-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f49e2-132">Request body</span></span>
<span data-ttu-id="f49e2-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f49e2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f49e2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f49e2-134">Response</span></span>

<span data-ttu-id="f49e2-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Schedule](../resources/schedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f49e2-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f49e2-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f49e2-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f49e2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f49e2-137">Request</span></span>

<span data-ttu-id="f49e2-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f49e2-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f49e2-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f49e2-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f49e2-140">C#</span><span class="sxs-lookup"><span data-stu-id="f49e2-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f49e2-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f49e2-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f49e2-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f49e2-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f49e2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f49e2-143">Response</span></span>

<span data-ttu-id="f49e2-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f49e2-144">The following is an example of the response.</span></span> 

><span data-ttu-id="f49e2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f49e2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
