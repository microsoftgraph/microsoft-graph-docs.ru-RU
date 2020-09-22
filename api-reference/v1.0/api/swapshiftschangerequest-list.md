---
title: Список Свапшифтсчанжерекуест
description: Получение списка объектов Свапшифтсчанжерекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 59e9b95d7619e0cff4ff26dabf95f2110c0cf4bd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970994"
---
# <a name="list-swapshiftschangerequest"></a><span data-ttu-id="2e81e-103">Список Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="2e81e-103">List swapShiftsChangeRequest</span></span>

<span data-ttu-id="2e81e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e81e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e81e-105">Получение списка объектов [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="2e81e-105">Retrieve a list of [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e81e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e81e-106">Permissions</span></span>

<span data-ttu-id="2e81e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e81e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e81e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e81e-109">Permission type</span></span>                        | <span data-ttu-id="2e81e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e81e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="2e81e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e81e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e81e-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2e81e-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e81e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e81e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e81e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e81e-114">Not supported.</span></span>    |
|<span data-ttu-id="2e81e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e81e-115">Application</span></span> | <span data-ttu-id="2e81e-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2e81e-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="2e81e-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="2e81e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2e81e-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="2e81e-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2e81e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e81e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e81e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e81e-120">Optional query parameters</span></span>

<span data-ttu-id="2e81e-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2e81e-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2e81e-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2e81e-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e81e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e81e-123">Request headers</span></span>

| <span data-ttu-id="2e81e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="2e81e-124">Name</span></span>      |<span data-ttu-id="2e81e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2e81e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e81e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e81e-126">Authorization</span></span> | <span data-ttu-id="2e81e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e81e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e81e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e81e-129">Request body</span></span>

<span data-ttu-id="2e81e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e81e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e81e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e81e-131">Response</span></span>

<span data-ttu-id="2e81e-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e81e-132">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e81e-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e81e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e81e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e81e-134">Request</span></span>

<span data-ttu-id="2e81e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e81e-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2e81e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e81e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests
```
# <a name="c"></a>[<span data-ttu-id="2e81e-137">C#</span><span class="sxs-lookup"><span data-stu-id="2e81e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e81e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e81e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e81e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e81e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e81e-140">Java</span><span class="sxs-lookup"><span data-stu-id="2e81e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-swapshiftschangerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="2e81e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e81e-141">Response</span></span>

<span data-ttu-id="2e81e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2e81e-142">The following is an example of the response.</span></span>

> <span data-ttu-id="2e81e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e81e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
        "id": "0b87dd20-d5ed-4764-9c3e-cfc8516def09",
        "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
        "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c",
        "assignedTo": "manager",
        "state": "approved",
        "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
        "senderDateTime": "2019-05-01T10:00:00Z",
        "senderMessage": "I can't make my shift, any chance we can swap?",
        "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
        "recipientActionDateTime": "2019-05-01T11:00:00Z",
        "recipientActionMessage": "Sure!",
        "managerUserId": "fdcc8d43-7f83-438a-9ab1-098e8f2a95ff",
        "managerActionDateTime": "2019-05-01T12:00:00Z",
        "managerActionMessage": "Approved!"
        }
    ]
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List swapShiftsChangeRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

