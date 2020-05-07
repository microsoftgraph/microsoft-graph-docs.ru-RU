---
title: Получение Опеншифт
description: Получение свойств и связей объекта опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c63c494f64930d96c7174d315bf271e4b07e7d7e
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155098"
---
# <a name="get-openshift"></a><span data-ttu-id="187ad-103">Получение Опеншифт</span><span class="sxs-lookup"><span data-stu-id="187ad-103">Get openShift</span></span>

<span data-ttu-id="187ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="187ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="187ad-105">Получение свойств и связей объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="187ad-105">Retrieve the properties and relationships of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="187ad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="187ad-106">Permissions</span></span>

<span data-ttu-id="187ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="187ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="187ad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="187ad-109">Permission type</span></span>                        | <span data-ttu-id="187ad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="187ad-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="187ad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="187ad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="187ad-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="187ad-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="187ad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="187ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="187ad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="187ad-114">Not supported.</span></span> |
| <span data-ttu-id="187ad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="187ad-115">Application</span></span>                            | <span data-ttu-id="187ad-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="187ad-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="187ad-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="187ad-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="187ad-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="187ad-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="187ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="187ad-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts/{openShiftId}
```
 
## <a name="request-headers"></a><span data-ttu-id="187ad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="187ad-120">Request headers</span></span>

| <span data-ttu-id="187ad-121">Имя</span><span class="sxs-lookup"><span data-stu-id="187ad-121">Name</span></span>      |<span data-ttu-id="187ad-122">Описание</span><span class="sxs-lookup"><span data-stu-id="187ad-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="187ad-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="187ad-123">Authorization</span></span> | <span data-ttu-id="187ad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="187ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="187ad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="187ad-126">Request body</span></span>

<span data-ttu-id="187ad-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="187ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="187ad-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="187ad-128">Response</span></span>

<span data-ttu-id="187ad-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [опеншифт](../resources/openshift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="187ad-129">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="187ad-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="187ad-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="187ad-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="187ad-131">Request</span></span>

<span data-ttu-id="187ad-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="187ad-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
---


### <a name="response"></a><span data-ttu-id="187ad-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="187ad-133">Response</span></span>

<span data-ttu-id="187ad-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="187ad-134">The following is an example of the response.</span></span>

> <span data-ttu-id="187ad-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="187ad-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":2,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T09:50:45.332Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T01:58:45.340Z",
  "code": "",
  "displayName": "Lunch"
  }
  ]
  },
  "draftOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":3,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.332Z",
  "endDateTime": "2018-10-04T08:58:45.340Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T07:58:45.332Z",
  "code": "Break",
  "displayName": "Lunch"
  }
  ]
  },
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
