---
title: Создание Опеншифт
description: Создайте экземпляр объекта опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5f9b02e5463c5215e67aef206d5876400ef275a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019952"
---
# <a name="create-openshift"></a><span data-ttu-id="38d2a-103">Создание Опеншифт</span><span class="sxs-lookup"><span data-stu-id="38d2a-103">Create openShift</span></span>

<span data-ttu-id="38d2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38d2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38d2a-105">Создайте экземпляр объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="38d2a-105">Create an instance of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="38d2a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38d2a-106">Permissions</span></span>

<span data-ttu-id="38d2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38d2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38d2a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38d2a-109">Permission type</span></span>                        | <span data-ttu-id="38d2a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38d2a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="38d2a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38d2a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="38d2a-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38d2a-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="38d2a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38d2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38d2a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38d2a-114">Not supported.</span></span> |
| <span data-ttu-id="38d2a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38d2a-115">Application</span></span>                            | <span data-ttu-id="38d2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38d2a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38d2a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38d2a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShifts
```

## <a name="request-headers"></a><span data-ttu-id="38d2a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38d2a-118">Request headers</span></span>

| <span data-ttu-id="38d2a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="38d2a-119">Name</span></span>      |<span data-ttu-id="38d2a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="38d2a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38d2a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38d2a-121">Authorization</span></span> | <span data-ttu-id="38d2a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38d2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38d2a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38d2a-124">Content-type</span></span> | <span data-ttu-id="38d2a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38d2a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38d2a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38d2a-127">Request body</span></span>

<span data-ttu-id="38d2a-128">Укажите новый объект [опеншифт](../resources/openshift.md) в тексте запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38d2a-128">Provide the new [openshift](../resources/openshift.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38d2a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="38d2a-129">Response</span></span>

<span data-ttu-id="38d2a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [опеншифт](../resources/openshift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38d2a-130">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38d2a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="38d2a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38d2a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="38d2a-132">Request</span></span>

<span data-ttu-id="38d2a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38d2a-133">The following is an example of the request.</span></span>
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
   "draftOpenShift":null,
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

### <a name="response"></a><span data-ttu-id="38d2a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="38d2a-134">Response</span></span>

<span data-ttu-id="38d2a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38d2a-135">The following is an example of the response.</span></span>

> <span data-ttu-id="38d2a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38d2a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "draftOpenShift": null,
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


