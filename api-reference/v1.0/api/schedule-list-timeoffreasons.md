---
title: Список Тимеоффреасонс
description: Получение списка Тимеоффреасонс по расписанию.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e2198026c4fa431cfd7e9395d552e64b79137e07
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155154"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="8adba-103">Список Тимеоффреасонс</span><span class="sxs-lookup"><span data-stu-id="8adba-103">List timeOffReasons</span></span>

<span data-ttu-id="8adba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8adba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8adba-105">Получение списка [тимеоффреасонс](../resources/timeoffreason.md) по [расписанию](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="8adba-105">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8adba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8adba-106">Permissions</span></span>

<span data-ttu-id="8adba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8adba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8adba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8adba-109">Permission type</span></span>      | <span data-ttu-id="8adba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8adba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8adba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8adba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8adba-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8adba-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8adba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8adba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8adba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8adba-114">Not supported.</span></span>    |
|<span data-ttu-id="8adba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8adba-115">Application</span></span> | <span data-ttu-id="8adba-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8adba-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="8adba-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="8adba-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8adba-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="8adba-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8adba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8adba-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="8adba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8adba-120">Request headers</span></span>

| <span data-ttu-id="8adba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8adba-121">Header</span></span>       | <span data-ttu-id="8adba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8adba-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8adba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8adba-123">Authorization</span></span>  | <span data-ttu-id="8adba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8adba-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8adba-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8adba-126">Request body</span></span>
<span data-ttu-id="8adba-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8adba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8adba-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8adba-128">Response</span></span>

<span data-ttu-id="8adba-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тимеоффреасон](../resources/timeoffreason.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8adba-129">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8adba-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8adba-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8adba-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8adba-131">Request</span></span>

<span data-ttu-id="8adba-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8adba-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons
```
---


#### <a name="response"></a><span data-ttu-id="8adba-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8adba-133">Response</span></span>

<span data-ttu-id="8adba-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8adba-134">The following is an example of the response.</span></span> 

><span data-ttu-id="8adba-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8adba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
      "createdDateTime": "2019-03-12T22:10:38.242Z",
      "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
      "displayName": "Vacation",
      "iconType": "plane",
      "isActive": true,
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of timeOffReason in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
