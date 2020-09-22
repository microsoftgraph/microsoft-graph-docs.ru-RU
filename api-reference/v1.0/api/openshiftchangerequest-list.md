---
title: Список Опеншифтчанжерекуестс
description: Получение списка объектов Опеншифтчанжерекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a4771862325c211b342e9985d586fbe50c29ba58
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059315"
---
# <a name="list-openshiftchangerequests"></a><span data-ttu-id="1ca46-103">Список Опеншифтчанжерекуестс</span><span class="sxs-lookup"><span data-stu-id="1ca46-103">List openShiftChangeRequests</span></span>

<span data-ttu-id="1ca46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ca46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1ca46-105">Получение списка объектов [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="1ca46-105">Retrieve a list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ca46-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca46-106">Permissions</span></span>

<span data-ttu-id="1ca46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ca46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ca46-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ca46-109">Permission type</span></span>                        | <span data-ttu-id="1ca46-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ca46-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ca46-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ca46-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ca46-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1ca46-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1ca46-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ca46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ca46-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ca46-114">Not supported.</span></span> |
| <span data-ttu-id="1ca46-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ca46-115">Application</span></span>                            | <span data-ttu-id="1ca46-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1ca46-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="1ca46-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="1ca46-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1ca46-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="1ca46-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1ca46-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ca46-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ca46-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1ca46-120">Optional query parameters</span></span>

<span data-ttu-id="1ca46-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1ca46-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1ca46-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1ca46-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ca46-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ca46-123">Request headers</span></span>

| <span data-ttu-id="1ca46-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1ca46-124">Name</span></span>      |<span data-ttu-id="1ca46-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1ca46-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1ca46-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ca46-126">Authorization</span></span> | <span data-ttu-id="1ca46-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ca46-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ca46-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ca46-129">Request body</span></span>

<span data-ttu-id="1ca46-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ca46-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ca46-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ca46-131">Response</span></span>

<span data-ttu-id="1ca46-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ca46-132">If successful, this method returns a `200 OK` response code and the list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ca46-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="1ca46-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ca46-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ca46-134">Request</span></span>

<span data-ttu-id="1ca46-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ca46-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="1ca46-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ca46-136">Response</span></span>

<span data-ttu-id="1ca46-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ca46-137">The following is an example of the response.</span></span>

> <span data-ttu-id="1ca46-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ca46-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [{
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
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

