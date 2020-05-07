---
title: Получение Тимеофф
description: Получение Тимеофф по ИДЕНТИФИКАТОРу.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2dc49bf529e6938ff297749f8acbc24584989318
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154915"
---
# <a name="get-timeoff"></a><span data-ttu-id="cae5a-103">Получение Тимеофф</span><span class="sxs-lookup"><span data-stu-id="cae5a-103">Get timeOff</span></span>

<span data-ttu-id="cae5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cae5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cae5a-105">Получение свойств и связей объекта [тимеофф](../resources/timeoff.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="cae5a-105">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="cae5a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae5a-106">Permissions</span></span>

<span data-ttu-id="cae5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae5a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae5a-109">Permission type</span></span>      | <span data-ttu-id="cae5a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cae5a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae5a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae5a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cae5a-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cae5a-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cae5a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae5a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae5a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae5a-114">Not supported.</span></span>    |
|<span data-ttu-id="cae5a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae5a-115">Application</span></span> | <span data-ttu-id="cae5a-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cae5a-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="cae5a-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="cae5a-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cae5a-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="cae5a-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cae5a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae5a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cae5a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cae5a-120">Optional query parameters</span></span>

<span data-ttu-id="cae5a-121">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cae5a-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cae5a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cae5a-122">Request headers</span></span>

| <span data-ttu-id="cae5a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cae5a-123">Header</span></span>       | <span data-ttu-id="cae5a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cae5a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cae5a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cae5a-125">Authorization</span></span>  | <span data-ttu-id="cae5a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cae5a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cae5a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cae5a-128">Request body</span></span>
<span data-ttu-id="cae5a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cae5a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cae5a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae5a-130">Response</span></span>

<span data-ttu-id="cae5a-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cae5a-131">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cae5a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cae5a-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cae5a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae5a-133">Request</span></span>

<span data-ttu-id="cae5a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae5a-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff/{timeOffId}
```
---


#### <a name="response"></a><span data-ttu-id="cae5a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae5a-135">Response</span></span>

<span data-ttu-id="cae5a-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cae5a-136">The following is an example of the response.</span></span> 

><span data-ttu-id="cae5a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cae5a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOff by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
