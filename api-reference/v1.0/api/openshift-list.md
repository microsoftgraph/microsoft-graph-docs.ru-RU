---
title: Список openShifts
description: Список объектов openshift в группе.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f5717a77c06c18e5ce36594eefcfd4130dbb8ce
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953504"
---
# <a name="list-openshifts"></a><span data-ttu-id="1bbf6-103">Список openShifts</span><span class="sxs-lookup"><span data-stu-id="1bbf6-103">List openShifts</span></span>

<span data-ttu-id="1bbf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bbf6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bbf6-105">Список [объектов openShift](../resources/openshift.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-105">List [openShift](../resources/openshift.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bbf6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bbf6-106">Permissions</span></span>

<span data-ttu-id="1bbf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bbf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1bbf6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bbf6-109">Permission type</span></span>                        | <span data-ttu-id="1bbf6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bbf6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1bbf6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bbf6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1bbf6-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bbf6-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1bbf6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bbf6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bbf6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-114">Not supported.</span></span> |
| <span data-ttu-id="1bbf6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bbf6-115">Application</span></span>                            | <span data-ttu-id="1bbf6-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bbf6-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="1bbf6-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1bbf6-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1bbf6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bbf6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1bbf6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1bbf6-120">Optional query parameters</span></span>

<span data-ttu-id="1bbf6-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1bbf6-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1bbf6-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="1bbf6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bbf6-123">Request headers</span></span>

| <span data-ttu-id="1bbf6-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1bbf6-124">Name</span></span>      |<span data-ttu-id="1bbf6-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1bbf6-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1bbf6-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bbf6-126">Authorization</span></span> | <span data-ttu-id="1bbf6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bbf6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bbf6-129">Request body</span></span>

<span data-ttu-id="1bbf6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bbf6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bbf6-131">Response</span></span>

<span data-ttu-id="1bbf6-132">В случае успешной работы этот метод возвращает код ответа и все `200 OK` [объекты openShift](../resources/openshift.md) в группе в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-132">If successful, this method returns a `200 OK` response code and all [openShift](../resources/openshift.md) objects in the team in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1bbf6-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="1bbf6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1bbf6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bbf6-134">Request</span></span>

<span data-ttu-id="1bbf6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1bbf6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bbf6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts
```
# <a name="c"></a>[<span data-ttu-id="1bbf6-137">C#</span><span class="sxs-lookup"><span data-stu-id="1bbf6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bbf6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bbf6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bbf6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bbf6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bbf6-140">Java</span><span class="sxs-lookup"><span data-stu-id="1bbf6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openshift-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="1bbf6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bbf6-141">Response</span></span>

<span data-ttu-id="1bbf6-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-142">The following is an example of the response.</span></span>

> <span data-ttu-id="1bbf6-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bbf6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

