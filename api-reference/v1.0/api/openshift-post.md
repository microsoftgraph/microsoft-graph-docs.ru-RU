---
title: Создание Опеншифт
description: Создайте экземпляр объекта Опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 44f9918b5a7a91b2a16f32f6c8c3970b003a5583
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155084"
---
# <a name="create-openshift"></a><span data-ttu-id="39e4b-103">Создание Опеншифт</span><span class="sxs-lookup"><span data-stu-id="39e4b-103">Create openShift</span></span>

<span data-ttu-id="39e4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39e4b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39e4b-105">Создайте экземпляр объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="39e4b-105">Create an instance of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39e4b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39e4b-106">Permissions</span></span>

<span data-ttu-id="39e4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39e4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39e4b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39e4b-109">Permission type</span></span>                        | <span data-ttu-id="39e4b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39e4b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39e4b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39e4b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39e4b-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="39e4b-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="39e4b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39e4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39e4b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39e4b-114">Not supported.</span></span> |
| <span data-ttu-id="39e4b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39e4b-115">Application</span></span>                            | <span data-ttu-id="39e4b-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39e4b-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="39e4b-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="39e4b-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="39e4b-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="39e4b-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="39e4b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39e4b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShifts
```
  
## <a name="request-headers"></a><span data-ttu-id="39e4b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39e4b-120">Request headers</span></span>

| <span data-ttu-id="39e4b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="39e4b-121">Name</span></span>      |<span data-ttu-id="39e4b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="39e4b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39e4b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39e4b-123">Authorization</span></span> | <span data-ttu-id="39e4b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39e4b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39e4b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39e4b-126">Content-type</span></span> | <span data-ttu-id="39e4b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39e4b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39e4b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39e4b-129">Request body</span></span>

<span data-ttu-id="39e4b-130">Укажите новый объект [опеншифт](../resources/openshift.md) в тексте запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39e4b-130">Provide the new [openShift](../resources/openshift.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39e4b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="39e4b-131">Response</span></span>

<span data-ttu-id="39e4b-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и созданный объект [опеншифт](../resources/openshift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39e4b-132">If successful, this method returns a `200 OK` response code and the created [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39e4b-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="39e4b-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39e4b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="39e4b-134">Request</span></span>

<span data-ttu-id="39e4b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39e4b-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openshifts
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

### <a name="response"></a><span data-ttu-id="39e4b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="39e4b-136">Response</span></span>

<span data-ttu-id="39e4b-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39e4b-137">The following is an example of the response.</span></span>

> <span data-ttu-id="39e4b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39e4b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
