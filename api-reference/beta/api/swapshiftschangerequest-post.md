---
title: Создание Свапшифтрекуест
description: Создайте экземпляр объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c4dd366ae1d9fc98cd495584581d3dfa0b73ab93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004426"
---
# <a name="create-swapshiftschangerequest"></a><span data-ttu-id="994f4-103">Создание Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="994f4-103">Create swapShiftsChangeRequest</span></span>

<span data-ttu-id="994f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="994f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="994f4-105">Создайте экземпляр объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="994f4-105">Create an instance of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="994f4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="994f4-106">Permissions</span></span>

<span data-ttu-id="994f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="994f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="994f4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="994f4-109">Permission type</span></span>                        | <span data-ttu-id="994f4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="994f4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="994f4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="994f4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="994f4-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="994f4-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="994f4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="994f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="994f4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="994f4-114">Not supported.</span></span> |
| <span data-ttu-id="994f4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="994f4-115">Application</span></span>                            | <span data-ttu-id="994f4-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="994f4-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="994f4-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="994f4-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="994f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="994f4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="994f4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="994f4-119">Optional query parameters</span></span>

<span data-ttu-id="994f4-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="994f4-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="994f4-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="994f4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="994f4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="994f4-122">Request headers</span></span>

| <span data-ttu-id="994f4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="994f4-123">Name</span></span>      |<span data-ttu-id="994f4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="994f4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="994f4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="994f4-125">Authorization</span></span> | <span data-ttu-id="994f4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="994f4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="994f4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="994f4-128">Content-type</span></span> | <span data-ttu-id="994f4-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="994f4-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="994f4-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="994f4-131">Request body</span></span>
<span data-ttu-id="994f4-132">В тексте запроса укажите представление объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="994f4-132">In the request body, provide a JSON representation of a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="994f4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="994f4-133">Response</span></span>

<span data-ttu-id="994f4-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и созданный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="994f4-134">If successful, this method returns a `200 OK` response code and the created [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="994f4-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="994f4-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="994f4-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="994f4-136">Request</span></span>

<span data-ttu-id="994f4-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="994f4-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="994f4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="994f4-138">Response</span></span>

<span data-ttu-id="994f4-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="994f4-139">The following is an example of the response.</span></span>

> <span data-ttu-id="994f4-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="994f4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


