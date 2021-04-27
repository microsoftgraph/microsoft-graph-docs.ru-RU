---
title: Get openShiftChangeRequest
description: Извлечение свойств и связей объекта openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 089fbd2096fff8bca2bb7cdff0d8502905dc5f3b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052077"
---
# <a name="get-openshiftchangerequest"></a><span data-ttu-id="75fe2-103">Get openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="75fe2-103">Get openShiftChangeRequest</span></span>

<span data-ttu-id="75fe2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75fe2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75fe2-105">Извлечение свойств и связей [объекта openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="75fe2-105">Retrieve the properties and relationships of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75fe2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75fe2-106">Permissions</span></span>

<span data-ttu-id="75fe2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75fe2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75fe2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75fe2-109">Permission type</span></span>                        | <span data-ttu-id="75fe2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75fe2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="75fe2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75fe2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="75fe2-112">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="75fe2-112">Group.ReadWrite.All, Group.Read.All</span></span> |
| <span data-ttu-id="75fe2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75fe2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75fe2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75fe2-114">Not supported.</span></span> |
| <span data-ttu-id="75fe2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75fe2-115">Application</span></span>                            | <span data-ttu-id="75fe2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75fe2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75fe2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75fe2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftChangeRequests/{openShiftsChangeRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75fe2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75fe2-118">Optional query parameters</span></span>

<span data-ttu-id="75fe2-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="75fe2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="75fe2-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="75fe2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="75fe2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75fe2-121">Request headers</span></span>

| <span data-ttu-id="75fe2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="75fe2-122">Name</span></span>      |<span data-ttu-id="75fe2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="75fe2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75fe2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75fe2-124">Authorization</span></span> | <span data-ttu-id="75fe2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75fe2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75fe2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75fe2-127">Request body</span></span>

<span data-ttu-id="75fe2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75fe2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75fe2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="75fe2-129">Response</span></span>

<span data-ttu-id="75fe2-130">В случае успеха этот метод возвращает код ответа и запрашивается `200 OK` [объект openShiftChangeRequest](../resources/openshiftchangerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75fe2-130">If successful, this method returns a `200 OK` response code and the requested [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75fe2-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="75fe2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75fe2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="75fe2-132">Request</span></span>

<span data-ttu-id="75fe2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75fe2-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75fe2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="75fe2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftChangeRequests/SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09
```
# <a name="c"></a>[<span data-ttu-id="75fe2-135">C#</span><span class="sxs-lookup"><span data-stu-id="75fe2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshiftchangerequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75fe2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75fe2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshiftchangerequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75fe2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75fe2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshiftchangerequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75fe2-138">Java</span><span class="sxs-lookup"><span data-stu-id="75fe2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openshiftchangerequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75fe2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="75fe2-139">Response</span></span>

<span data-ttu-id="75fe2-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75fe2-140">The following is an example of the response.</span></span>

> <span data-ttu-id="75fe2-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75fe2-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "assignedTo": "manager",
  "state": "pending",
  "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
  "senderDateTime": "2019-05-01T10:00:00Z",
  "senderMessage": "Can I take this shift?",
  "managerUserId": null,
  "managerActionDateTime": null,
  "managerActionMessage": null,
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
  "description": "Get openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


