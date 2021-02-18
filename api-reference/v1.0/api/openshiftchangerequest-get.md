---
title: Get openShiftChangeRequest
description: Извлечение свойств и связей объекта openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6cb69d55bf7a0197f2cb06f4a97776a035f58a03
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292597"
---
# <a name="get-openshiftchangerequest"></a><span data-ttu-id="ad5b9-103">Get openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="ad5b9-103">Get openShiftChangeRequest</span></span>

<span data-ttu-id="ad5b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad5b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad5b9-105">Извлечение свойств и связей объекта [openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="ad5b9-105">Retrieve the properties and relationships of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad5b9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad5b9-106">Permissions</span></span>

<span data-ttu-id="ad5b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad5b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad5b9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad5b9-109">Permission type</span></span>                        | <span data-ttu-id="ad5b9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad5b9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ad5b9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad5b9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad5b9-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad5b9-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ad5b9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad5b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad5b9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-114">Not supported.</span></span> |
| <span data-ttu-id="ad5b9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad5b9-115">Application</span></span>                            | <span data-ttu-id="ad5b9-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad5b9-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="ad5b9-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ad5b9-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ad5b9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad5b9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftChangeRequests/{openShiftsChangeRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad5b9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad5b9-120">Optional query parameters</span></span>

<span data-ttu-id="ad5b9-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ad5b9-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ad5b9-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad5b9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad5b9-123">Request headers</span></span>

| <span data-ttu-id="ad5b9-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ad5b9-124">Name</span></span>      |<span data-ttu-id="ad5b9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ad5b9-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad5b9-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad5b9-126">Authorization</span></span> | <span data-ttu-id="ad5b9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad5b9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad5b9-129">Request body</span></span>

<span data-ttu-id="ad5b9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad5b9-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad5b9-131">Response</span></span>

<span data-ttu-id="ad5b9-132">В случае успеха этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [openShiftChangeRequest](../resources/openshiftchangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-132">If successful, this method returns a `200 OK` response code and the requested [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad5b9-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="ad5b9-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ad5b9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad5b9-134">Request</span></span>

<span data-ttu-id="ad5b9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftChangeRequests/SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09
```

### <a name="response"></a><span data-ttu-id="ad5b9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad5b9-136">Response</span></span>

<span data-ttu-id="ad5b9-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ad5b9-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad5b9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

