---
title: Список Свапшифтсчанжерекуест
description: Получение списка объектов Свапшифтсчанжерекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 70a14c64ce697d8440292eeb773447961ae76347
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971942"
---
# <a name="list-swapshiftschangerequest"></a><span data-ttu-id="d4310-103">Список Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="d4310-103">List swapShiftsChangeRequest</span></span>

<span data-ttu-id="d4310-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4310-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4310-105">Получение списка объектов [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="d4310-105">Retrieve a list of [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4310-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4310-106">Permissions</span></span>

<span data-ttu-id="d4310-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4310-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4310-109">Permission type</span></span>                        | <span data-ttu-id="d4310-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4310-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4310-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4310-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4310-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4310-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d4310-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4310-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4310-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4310-114">Not supported.</span></span> |
| <span data-ttu-id="d4310-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d4310-115">Application</span></span> | <span data-ttu-id="d4310-116">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="d4310-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="d4310-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="d4310-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="d4310-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4310-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4310-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d4310-119">Optional query parameters</span></span>

<span data-ttu-id="d4310-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d4310-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d4310-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d4310-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4310-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4310-122">Request headers</span></span>

| <span data-ttu-id="d4310-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d4310-123">Name</span></span>      |<span data-ttu-id="d4310-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d4310-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4310-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4310-125">Authorization</span></span> | <span data-ttu-id="d4310-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4310-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4310-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4310-128">Request body</span></span>

<span data-ttu-id="d4310-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4310-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4310-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4310-130">Response</span></span>

<span data-ttu-id="d4310-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4310-131">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4310-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4310-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4310-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4310-133">Request</span></span>

<span data-ttu-id="d4310-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4310-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4310-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4310-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/swapShiftsChangeRequests
```
# <a name="c"></a>[<span data-ttu-id="d4310-136">C#</span><span class="sxs-lookup"><span data-stu-id="d4310-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4310-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4310-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4310-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4310-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4310-139">Java</span><span class="sxs-lookup"><span data-stu-id="d4310-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-swapshiftschangerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4310-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4310-140">Response</span></span>

<span data-ttu-id="d4310-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4310-141">The following is an example of the response.</span></span>

> <span data-ttu-id="d4310-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4310-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


