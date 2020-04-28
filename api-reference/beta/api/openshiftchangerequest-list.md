---
title: Список Опеншифтчанжерекуестс
description: Получение списка объектов Опеншифтчанжерекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e9f39258ec4aa202053c5979658e70e352a38f20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456378"
---
# <a name="list-openshiftchangerequests"></a><span data-ttu-id="3a1ab-103">Список Опеншифтчанжерекуестс</span><span class="sxs-lookup"><span data-stu-id="3a1ab-103">List openShiftChangeRequests</span></span>

<span data-ttu-id="3a1ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a1ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a1ab-105">Получение списка объектов [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-105">Retrieve a list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a1ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a1ab-106">Permissions</span></span>

<span data-ttu-id="3a1ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a1ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a1ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a1ab-109">Permission type</span></span>                        | <span data-ttu-id="3a1ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a1ab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3a1ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a1ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a1ab-112">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3a1ab-112">Group.ReadWrite.All, Group.Read.All</span></span> |
| <span data-ttu-id="3a1ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a1ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a1ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-114">Not supported.</span></span> |
| <span data-ttu-id="3a1ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a1ab-115">Application</span></span>                            | <span data-ttu-id="3a1ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a1ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a1ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a1ab-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a1ab-118">Optional query parameters</span></span>

<span data-ttu-id="3a1ab-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3a1ab-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3a1ab-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a1ab-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a1ab-121">Request headers</span></span>

| <span data-ttu-id="3a1ab-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3a1ab-122">Name</span></span>      |<span data-ttu-id="3a1ab-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3a1ab-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a1ab-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a1ab-124">Authorization</span></span> | <span data-ttu-id="3a1ab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a1ab-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a1ab-127">Request body</span></span>

<span data-ttu-id="3a1ab-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a1ab-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a1ab-129">Response</span></span>

<span data-ttu-id="3a1ab-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-130">If successful, this method returns a `200 OK` response code and the list of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a1ab-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a1ab-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a1ab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a1ab-132">Request</span></span>

<span data-ttu-id="3a1ab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="3a1ab-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a1ab-134">Response</span></span>

<span data-ttu-id="3a1ab-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-135">The following is an example of the response.</span></span>

> <span data-ttu-id="3a1ab-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a1ab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
