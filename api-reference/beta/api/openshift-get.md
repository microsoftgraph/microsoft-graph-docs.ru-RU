---
title: Get openShift
description: Извлечение свойств и связей объекта openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5ba72fec21d76458b256ef46a88f4136886631b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050110"
---
# <a name="get-openshift"></a><span data-ttu-id="642b5-103">Get openShift</span><span class="sxs-lookup"><span data-stu-id="642b5-103">Get openShift</span></span>

<span data-ttu-id="642b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="642b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="642b5-105">Извлечение свойств и связей объекта [openshift.](../resources/openshift.md)</span><span class="sxs-lookup"><span data-stu-id="642b5-105">Retrieve the properties and relationships of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="642b5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="642b5-106">Permissions</span></span>

<span data-ttu-id="642b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="642b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="642b5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="642b5-109">Permission type</span></span>                        | <span data-ttu-id="642b5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="642b5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="642b5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="642b5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="642b5-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642b5-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="642b5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="642b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="642b5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="642b5-114">Not supported.</span></span> |
| <span data-ttu-id="642b5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="642b5-115">Application</span></span>                            | <span data-ttu-id="642b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="642b5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="642b5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="642b5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="642b5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="642b5-118">Optional query parameters</span></span>

<span data-ttu-id="642b5-119">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="642b5-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="642b5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="642b5-120">Request headers</span></span>

| <span data-ttu-id="642b5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="642b5-121">Name</span></span>      |<span data-ttu-id="642b5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="642b5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="642b5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="642b5-123">Authorization</span></span> | <span data-ttu-id="642b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="642b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="642b5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="642b5-126">Request body</span></span>

<span data-ttu-id="642b5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="642b5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="642b5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="642b5-128">Response</span></span>

<span data-ttu-id="642b5-129">В случае успешной работы этот метод возвращает код ответа и запрашиваемого `200 OK` [объекта openShift](../resources/openshift.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="642b5-129">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="642b5-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="642b5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="642b5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="642b5-131">Request</span></span>

<span data-ttu-id="642b5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="642b5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="642b5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="642b5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="642b5-134">C#</span><span class="sxs-lookup"><span data-stu-id="642b5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="642b5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="642b5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="642b5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="642b5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="642b5-137">Java</span><span class="sxs-lookup"><span data-stu-id="642b5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openshift-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="642b5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="642b5-138">Response</span></span>

<span data-ttu-id="642b5-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="642b5-139">The following is an example of the response.</span></span>

> <span data-ttu-id="642b5-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="642b5-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


