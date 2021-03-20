---
title: Get openShift
description: Извлечение свойств и связей объекта openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ae5baeb3fb01902d89e9e9c72e948c4aef2e9212
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953521"
---
# <a name="get-openshift"></a><span data-ttu-id="a36f0-103">Get openShift</span><span class="sxs-lookup"><span data-stu-id="a36f0-103">Get openShift</span></span>

<span data-ttu-id="a36f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a36f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a36f0-105">Извлечение свойств и связей объекта [openshift.](../resources/openshift.md)</span><span class="sxs-lookup"><span data-stu-id="a36f0-105">Retrieve the properties and relationships of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a36f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a36f0-106">Permissions</span></span>

<span data-ttu-id="a36f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a36f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a36f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a36f0-109">Permission type</span></span>                        | <span data-ttu-id="a36f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a36f0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a36f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a36f0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a36f0-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a36f0-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a36f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a36f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a36f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a36f0-114">Not supported.</span></span> |
| <span data-ttu-id="a36f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a36f0-115">Application</span></span>                            | <span data-ttu-id="a36f0-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a36f0-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="a36f0-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a36f0-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a36f0-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="a36f0-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a36f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a36f0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a36f0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a36f0-120">Optional query parameters</span></span>

<span data-ttu-id="a36f0-121">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a36f0-121">This method does not support OData query parameters to customize the response.</span></span>
 
## <a name="request-headers"></a><span data-ttu-id="a36f0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a36f0-122">Request headers</span></span>

| <span data-ttu-id="a36f0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a36f0-123">Name</span></span>      |<span data-ttu-id="a36f0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a36f0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a36f0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a36f0-125">Authorization</span></span> | <span data-ttu-id="a36f0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a36f0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a36f0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a36f0-128">Request body</span></span>

<span data-ttu-id="a36f0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a36f0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a36f0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a36f0-130">Response</span></span>

<span data-ttu-id="a36f0-131">В случае успешной работы этот метод возвращает код ответа и запрашиваемого `200 OK` [объекта openShift](../resources/openshift.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a36f0-131">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a36f0-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="a36f0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a36f0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a36f0-133">Request</span></span>

<span data-ttu-id="a36f0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a36f0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a36f0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a36f0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="a36f0-136">C#</span><span class="sxs-lookup"><span data-stu-id="a36f0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a36f0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a36f0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a36f0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a36f0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a36f0-139">Java</span><span class="sxs-lookup"><span data-stu-id="a36f0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openshift-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="a36f0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a36f0-140">Response</span></span>

<span data-ttu-id="a36f0-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a36f0-141">The following is an example of the response.</span></span>

> <span data-ttu-id="a36f0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a36f0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

