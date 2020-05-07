---
title: Создание Свапшифтрекуест
description: Создайте экземпляр объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fae65ef9812b68bea46960966af7caf694cb3b37
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155021"
---
# <a name="create-swapshiftschangerequest"></a><span data-ttu-id="23791-103">Создание Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="23791-103">Create swapShiftsChangeRequest</span></span>

<span data-ttu-id="23791-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23791-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23791-105">Создайте экземпляр объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="23791-105">Create an instance of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23791-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23791-106">Permissions</span></span>

<span data-ttu-id="23791-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23791-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23791-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23791-109">Permission type</span></span>                        | <span data-ttu-id="23791-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23791-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="23791-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23791-111">Delegated (work or school account)</span></span> |<span data-ttu-id="23791-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="23791-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="23791-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23791-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23791-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23791-114">Not supported.</span></span>    |
|<span data-ttu-id="23791-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23791-115">Application</span></span> | <span data-ttu-id="23791-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23791-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="23791-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="23791-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="23791-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="23791-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="23791-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23791-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23791-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23791-120">Optional query parameters</span></span>

<span data-ttu-id="23791-121">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23791-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="23791-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="23791-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="23791-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23791-123">Request headers</span></span>

| <span data-ttu-id="23791-124">Имя</span><span class="sxs-lookup"><span data-stu-id="23791-124">Name</span></span>      |<span data-ttu-id="23791-125">Описание</span><span class="sxs-lookup"><span data-stu-id="23791-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23791-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23791-126">Authorization</span></span> | <span data-ttu-id="23791-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23791-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23791-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23791-129">Content-type</span></span> | <span data-ttu-id="23791-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23791-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23791-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23791-132">Request body</span></span>
<span data-ttu-id="23791-133">В тексте запроса укажите представление объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23791-133">In the request body, provide a JSON representation of a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="23791-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="23791-134">Response</span></span>

<span data-ttu-id="23791-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и созданный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23791-135">If successful, this method returns a `200 OK` response code and the created [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23791-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="23791-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23791-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="23791-137">Request</span></span>

<span data-ttu-id="23791-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23791-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/swapShiftsChangeRequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
  "senderMessage": "I can't make my shift, any chance we can swap?",
  "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
  "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c"
}
```

### <a name="response"></a><span data-ttu-id="23791-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="23791-139">Response</span></span>

<span data-ttu-id="23791-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23791-140">The following is an example of the response.</span></span>

> <span data-ttu-id="23791-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23791-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
