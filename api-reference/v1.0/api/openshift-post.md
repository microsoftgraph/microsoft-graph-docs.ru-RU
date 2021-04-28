---
title: Создание openShift
description: Создание экземпляра объекта openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6109cbc84e3eeb5f1bb6e627b985225d77f0436
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051335"
---
# <a name="create-openshift"></a><span data-ttu-id="60af3-103">Создание openShift</span><span class="sxs-lookup"><span data-stu-id="60af3-103">Create openShift</span></span>

<span data-ttu-id="60af3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60af3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60af3-105">Создание экземпляра [объекта openShift.](../resources/openshift.md)</span><span class="sxs-lookup"><span data-stu-id="60af3-105">Create an instance of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60af3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60af3-106">Permissions</span></span>

<span data-ttu-id="60af3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60af3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60af3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60af3-109">Permission type</span></span>                        | <span data-ttu-id="60af3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60af3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="60af3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60af3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="60af3-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60af3-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="60af3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60af3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60af3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60af3-114">Not supported.</span></span> |
| <span data-ttu-id="60af3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60af3-115">Application</span></span>                            | <span data-ttu-id="60af3-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60af3-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="60af3-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="60af3-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="60af3-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="60af3-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="60af3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60af3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShifts
```
  
## <a name="request-headers"></a><span data-ttu-id="60af3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60af3-120">Request headers</span></span>

| <span data-ttu-id="60af3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="60af3-121">Name</span></span>      |<span data-ttu-id="60af3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="60af3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60af3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60af3-123">Authorization</span></span> | <span data-ttu-id="60af3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60af3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60af3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60af3-126">Content-type</span></span> | <span data-ttu-id="60af3-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60af3-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60af3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60af3-129">Request body</span></span>

<span data-ttu-id="60af3-130">Предокажи новый [объект openShift](../resources/openshift.md) в теле запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60af3-130">Provide the new [openShift](../resources/openshift.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60af3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="60af3-131">Response</span></span>

<span data-ttu-id="60af3-132">В случае успешной работы этот метод возвращает код ответа и созданный `200 OK` [объект openShift](../resources/openshift.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="60af3-132">If successful, this method returns a `200 OK` response code and the created [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60af3-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="60af3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60af3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="60af3-134">Request</span></span>

<span data-ttu-id="60af3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60af3-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="60af3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="60af3-136">Response</span></span>

<span data-ttu-id="60af3-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="60af3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="60af3-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="60af3-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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

