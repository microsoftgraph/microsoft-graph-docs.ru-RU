---
title: Получение Свапшифтсчанжерекуест
description: Получение свойств и связей объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5203f7902a5c25683e173c4647b7cb776655e05c
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951754"
---
# <a name="get-swapshiftschangerequest"></a><span data-ttu-id="cecbb-103">Получение Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="cecbb-103">Get swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cecbb-104">Получение свойств и связей объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="cecbb-104">Retrieve the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cecbb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cecbb-105">Permissions</span></span>

<span data-ttu-id="cecbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cecbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cecbb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cecbb-108">Permission type</span></span>                        | <span data-ttu-id="cecbb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cecbb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cecbb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cecbb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cecbb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cecbb-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cecbb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cecbb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cecbb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cecbb-113">Not supported.</span></span> |
| <span data-ttu-id="cecbb-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="cecbb-114">Application</span></span> | <span data-ttu-id="cecbb-115">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="cecbb-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="cecbb-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="cecbb-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="cecbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cecbb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cecbb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cecbb-118">Optional query parameters</span></span>

<span data-ttu-id="cecbb-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cecbb-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cecbb-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cecbb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cecbb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cecbb-121">Request headers</span></span>

| <span data-ttu-id="cecbb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cecbb-122">Name</span></span>      |<span data-ttu-id="cecbb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cecbb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cecbb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cecbb-124">Authorization</span></span> | <span data-ttu-id="cecbb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cecbb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cecbb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cecbb-127">Request body</span></span>

<span data-ttu-id="cecbb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cecbb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cecbb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cecbb-129">Response</span></span>

<span data-ttu-id="cecbb-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cecbb-130">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cecbb-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="cecbb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cecbb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cecbb-132">Request</span></span>

<span data-ttu-id="cecbb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cecbb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}
```

### <a name="response"></a><span data-ttu-id="cecbb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cecbb-134">Response</span></span>

<span data-ttu-id="cecbb-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cecbb-135">The following is an example of the response.</span></span>

> <span data-ttu-id="cecbb-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cecbb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
