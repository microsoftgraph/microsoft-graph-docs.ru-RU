---
title: Создание Опеншифт
description: Создайте экземпляр объекта опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 635dd4c81e0b7f6cbe0cd2ceb26e391f2fb3bac5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952225"
---
# <a name="create-openshift"></a><span data-ttu-id="474ec-103">Создание Опеншифт</span><span class="sxs-lookup"><span data-stu-id="474ec-103">Create openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="474ec-104">Создайте экземпляр объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="474ec-104">Create an instance of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="474ec-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="474ec-105">Permissions</span></span>

<span data-ttu-id="474ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="474ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="474ec-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="474ec-108">Permission type</span></span>                        | <span data-ttu-id="474ec-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="474ec-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="474ec-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="474ec-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="474ec-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474ec-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="474ec-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="474ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="474ec-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="474ec-113">Not supported.</span></span> |
| <span data-ttu-id="474ec-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="474ec-114">Application</span></span>                            | <span data-ttu-id="474ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="474ec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="474ec-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="474ec-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="474ec-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="474ec-117">Optional query parameters</span></span>

<span data-ttu-id="474ec-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="474ec-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="474ec-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="474ec-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="474ec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="474ec-120">Request headers</span></span>

| <span data-ttu-id="474ec-121">Имя</span><span class="sxs-lookup"><span data-stu-id="474ec-121">Name</span></span>      |<span data-ttu-id="474ec-122">Описание</span><span class="sxs-lookup"><span data-stu-id="474ec-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="474ec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="474ec-123">Authorization</span></span> | <span data-ttu-id="474ec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="474ec-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="474ec-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="474ec-126">Content-type</span></span> | <span data-ttu-id="474ec-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="474ec-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="474ec-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="474ec-129">Request body</span></span>

<span data-ttu-id="474ec-130">Укажите новый объект [опеншифт](../resources/openshift.md) в тексте запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="474ec-130">Provide the new [openshift](../resources/openshift.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="474ec-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="474ec-131">Response</span></span>

<span data-ttu-id="474ec-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [опеншифт](../resources/openshift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="474ec-132">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="474ec-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="474ec-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="474ec-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="474ec-134">Request</span></span>

<span data-ttu-id="474ec-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="474ec-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openshifts
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
   "id":"OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
   "schedulingGroupId":"TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
   "sharedOpenShift":{
      "notes":"InventoryManagement",
      "openSlotCount":2,
      "displayName":"Dayshift",
      "startDateTime":"2018-10-04T00: 58: 45.340Z",
      "endDateTime":"2018-10-04T09: 50: 45.332Z",
      "theme":"white",
      "activities":[
         {
            "isPaid":true,
            "startDateTime":"2018-10-04T00: 58: 45.340Z",
            "endDateTime":"2018-10-04T01: 58: 45.340Z",
            "code":"",
            "displayName":"Lunch"
         }
      ]
   },
   "draftOpenShift":{
      "notes":"InventoryManagement",
      "openSlotCount":3,
      "displayName":"Dayshift",
      "startDateTime":"2018-10-04T00: 58: 45.332Z",
      "endDateTime":"2018-10-04T08: 58: 45.340Z",
      "theme":"white",
      "activities":[
         {
            "isPaid":true,
            "startDateTime":"2018-10-04T00: 58: 45.340Z",
            "endDateTime":"2018-10-04T07: 58: 45.332Z",
            "code":"Break",
            "displayName":"Lunch"
         }
      ]
   },
   "createdDateTime":"2019-03-14T04: 32: 51.451Z",
   "lastModifiedDateTime":"2019-03-14T05: 32: 51.451Z",
   "lastModifiedBy":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
         "displayName":"JohnDoe"
      }
   }
}
```

### <a name="response"></a><span data-ttu-id="474ec-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="474ec-136">Response</span></span>

<span data-ttu-id="474ec-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="474ec-137">The following is an example of the response.</span></span>

> <span data-ttu-id="474ec-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="474ec-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
