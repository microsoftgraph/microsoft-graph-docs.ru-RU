---
title: Получение Опеншифтчанжерекуест
description: Получение свойств и связей объекта Опеншифтчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6a2f7e9f55afc566590a847fe8542ae062b182cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456376"
---
# <a name="get-openshiftchangerequest"></a><span data-ttu-id="313a3-103">Получение Опеншифтчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="313a3-103">Get openShiftChangeRequest</span></span>

<span data-ttu-id="313a3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="313a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="313a3-105">Получение свойств и связей объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="313a3-105">Retrieve the properties and relationships of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="313a3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="313a3-106">Permissions</span></span>

<span data-ttu-id="313a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="313a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="313a3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="313a3-109">Permission type</span></span>                        | <span data-ttu-id="313a3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="313a3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="313a3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="313a3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="313a3-112">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="313a3-112">Group.ReadWrite.All, Group.Read.All</span></span> |
| <span data-ttu-id="313a3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="313a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="313a3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="313a3-114">Not supported.</span></span> |
| <span data-ttu-id="313a3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="313a3-115">Application</span></span>                            | <span data-ttu-id="313a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="313a3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="313a3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="313a3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftsChangeRequests/{openShiftsChangeRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="313a3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="313a3-118">Optional query parameters</span></span>

<span data-ttu-id="313a3-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="313a3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="313a3-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="313a3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="313a3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="313a3-121">Request headers</span></span>

| <span data-ttu-id="313a3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="313a3-122">Name</span></span>      |<span data-ttu-id="313a3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="313a3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="313a3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="313a3-124">Authorization</span></span> | <span data-ttu-id="313a3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="313a3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="313a3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="313a3-127">Request body</span></span>

<span data-ttu-id="313a3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="313a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="313a3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="313a3-129">Response</span></span>

<span data-ttu-id="313a3-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="313a3-130">If successful, this method returns a `200 OK` response code and the requested [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="313a3-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="313a3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="313a3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="313a3-132">Request</span></span>

<span data-ttu-id="313a3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="313a3-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09
```

### <a name="response"></a><span data-ttu-id="313a3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="313a3-134">Response</span></span>

<span data-ttu-id="313a3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="313a3-135">The following is an example of the response.</span></span>

> <span data-ttu-id="313a3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="313a3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
