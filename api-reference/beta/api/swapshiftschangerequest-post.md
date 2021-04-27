---
title: Создание swapshiftRequest
description: Создание экземпляра swapShiftsChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b1f873194d18f3ec34681f90942d5de2cbb089b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054835"
---
# <a name="create-swapshiftschangerequest"></a><span data-ttu-id="73d8d-103">Создание swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="73d8d-103">Create swapShiftsChangeRequest</span></span>

<span data-ttu-id="73d8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73d8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73d8d-105">Создайте экземпляр объекта [swapShiftsChangeRequest.](../resources/swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="73d8d-105">Create an instance of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73d8d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73d8d-106">Permissions</span></span>

<span data-ttu-id="73d8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73d8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73d8d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73d8d-109">Permission type</span></span>                        | <span data-ttu-id="73d8d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73d8d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="73d8d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73d8d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="73d8d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73d8d-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="73d8d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73d8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73d8d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73d8d-114">Not supported.</span></span> |
| <span data-ttu-id="73d8d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="73d8d-115">Application</span></span>                            | <span data-ttu-id="73d8d-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="73d8d-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="73d8d-117">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="73d8d-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="73d8d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73d8d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73d8d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73d8d-119">Optional query parameters</span></span>

<span data-ttu-id="73d8d-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="73d8d-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="73d8d-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="73d8d-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="73d8d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73d8d-122">Request headers</span></span>

| <span data-ttu-id="73d8d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="73d8d-123">Name</span></span>      |<span data-ttu-id="73d8d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="73d8d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73d8d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73d8d-125">Authorization</span></span> | <span data-ttu-id="73d8d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73d8d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73d8d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73d8d-128">Content-type</span></span> | <span data-ttu-id="73d8d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73d8d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73d8d-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73d8d-131">Request body</span></span>
<span data-ttu-id="73d8d-132">В теле запроса предостерегать представление JSON нового [объекта swapShiftsChangeRequest.](../resources/swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="73d8d-132">In the request body, provide a JSON representation of a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="73d8d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="73d8d-133">Response</span></span>

<span data-ttu-id="73d8d-134">В случае успешной работы этот метод возвращает код ответа и созданный `200 OK` [объект swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="73d8d-134">If successful, this method returns a `200 OK` response code and the created [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73d8d-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="73d8d-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73d8d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="73d8d-136">Request</span></span>

<span data-ttu-id="73d8d-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73d8d-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73d8d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="73d8d-138">Response</span></span>

<span data-ttu-id="73d8d-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="73d8d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="73d8d-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="73d8d-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


