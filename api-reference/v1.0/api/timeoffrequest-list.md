---
title: Список Тимеоффрекуест
description: Получение списка объектов Тимеоффрекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ab16c23d1535cd8b67d20a9dcee97ca42031dda1
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154285"
---
# <a name="list-timeoffrequest"></a><span data-ttu-id="6c470-103">Список Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="6c470-103">List timeOffRequest</span></span>

<span data-ttu-id="6c470-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c470-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c470-105">Получение списка объектов [тимеоффрекуест](../resources/timeoffrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="6c470-105">Retrieve a list of [timeOffRequest](../resources/timeoffrequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c470-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c470-106">Permissions</span></span>

<span data-ttu-id="6c470-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c470-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c470-109">Permission type</span></span>                        | <span data-ttu-id="6c470-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c470-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="6c470-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c470-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6c470-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c470-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c470-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c470-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c470-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c470-114">Not supported.</span></span>    |
|<span data-ttu-id="6c470-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c470-115">Application</span></span> | <span data-ttu-id="6c470-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c470-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="6c470-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="6c470-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6c470-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="6c470-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="6c470-119">в настоящее время только частный предварительный просмотр и недоступно для общедоступного использования.</span><span class="sxs-lookup"><span data-stu-id="6c470-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="6c470-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c470-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c470-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6c470-121">Optional query parameters</span></span>

<span data-ttu-id="6c470-122">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6c470-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6c470-123">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6c470-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c470-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c470-124">Request headers</span></span>

| <span data-ttu-id="6c470-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6c470-125">Name</span></span>      |<span data-ttu-id="6c470-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6c470-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6c470-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c470-127">Authorization</span></span> | <span data-ttu-id="6c470-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c470-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c470-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c470-130">Request body</span></span>

<span data-ttu-id="6c470-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c470-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c470-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c470-132">Response</span></span>

<span data-ttu-id="6c470-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенные объекты [тимеоффрекуест](../resources/timeoffrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c470-133">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c470-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c470-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c470-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c470-135">Request</span></span>

<span data-ttu-id="6c470-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c470-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests
```
---

### <a name="response"></a><span data-ttu-id="6c470-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c470-137">Response</span></span>

<span data-ttu-id="6c470-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c470-138">The following is an example of the response.</span></span>

> <span data-ttu-id="6c470-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c470-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        {
        "id": "0b87dd20-d5ed-4764-9c3e-cfc8516def09",
        "startDateTime": "datetime-value",
        "endDateTime": "datetime-value",
        "timeOffReasonId": "timeOffReasonId-value"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
