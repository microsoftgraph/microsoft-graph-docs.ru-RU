---
title: Создание Свапшифтрекуест
description: Создайте экземпляр объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ee4e9dcf16489952de2c516a5247d4bb2d6d3f39
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952092"
---
# <a name="create-swapshiftschangerequest"></a><span data-ttu-id="59dd8-103">Создание Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="59dd8-103">Create swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59dd8-104">Создайте экземпляр объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="59dd8-104">Create an instance of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59dd8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59dd8-105">Permissions</span></span>

<span data-ttu-id="59dd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59dd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59dd8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59dd8-108">Permission type</span></span>                        | <span data-ttu-id="59dd8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59dd8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="59dd8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59dd8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="59dd8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59dd8-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="59dd8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59dd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59dd8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59dd8-113">Not supported.</span></span> |
| <span data-ttu-id="59dd8-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="59dd8-114">Application</span></span>                            | <span data-ttu-id="59dd8-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="59dd8-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="59dd8-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="59dd8-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="59dd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59dd8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59dd8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="59dd8-118">Optional query parameters</span></span>

<span data-ttu-id="59dd8-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="59dd8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="59dd8-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="59dd8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="59dd8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59dd8-121">Request headers</span></span>

| <span data-ttu-id="59dd8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="59dd8-122">Name</span></span>      |<span data-ttu-id="59dd8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="59dd8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59dd8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59dd8-124">Authorization</span></span> | <span data-ttu-id="59dd8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59dd8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59dd8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59dd8-127">Content-type</span></span> | <span data-ttu-id="59dd8-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59dd8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59dd8-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="59dd8-130">Request body</span></span>
<span data-ttu-id="59dd8-131">В тексте запроса укажите представление объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59dd8-131">In the request body, provide a JSON representation of a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="59dd8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="59dd8-132">Response</span></span>

<span data-ttu-id="59dd8-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и созданный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59dd8-133">If successful, this method returns a `200 OK` response code and the created [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59dd8-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="59dd8-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59dd8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="59dd8-135">Request</span></span>

<span data-ttu-id="59dd8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59dd8-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/swapShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
  "senderMessage": "I can't make my shift, any chance we can swap?",
  "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
  "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c"
}
```

### <a name="response"></a><span data-ttu-id="59dd8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="59dd8-137">Response</span></span>

<span data-ttu-id="59dd8-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="59dd8-138">The following is an example of the response.</span></span>

> <span data-ttu-id="59dd8-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59dd8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
"assignedTo": "recipient",
"state": "pending",
"senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
"senderDateTime": "2019-05-01T10:00:00Z",
"senderMessage": "I can't make my shift, any chance we can swap?",
"recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
"recipientActionDateTime": null,
"recipientActionMessage": null,
"managerUserId": null,
"managerActionDateTime": null,
"managerActionMessage": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create swapShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
