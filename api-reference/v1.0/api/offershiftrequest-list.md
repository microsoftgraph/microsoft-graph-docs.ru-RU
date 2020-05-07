---
title: Список Оффершифтрекуест
description: Получение свойств и связей всех объектов Оффершифтрекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9b2c722b3217395928fb6a60d29d6e43b6d36792
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154930"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="08d73-103">Список Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="08d73-103">List offerShiftRequest</span></span>

<span data-ttu-id="08d73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08d73-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08d73-105">Получение свойств и связей всех объектов [оффершифтрекуест](../resources/offershiftrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="08d73-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="08d73-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08d73-106">Permissions</span></span>

<span data-ttu-id="08d73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08d73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08d73-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08d73-109">Permission type</span></span>                        | <span data-ttu-id="08d73-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08d73-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="08d73-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08d73-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08d73-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="08d73-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="08d73-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08d73-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08d73-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08d73-114">Not supported.</span></span> |
| <span data-ttu-id="08d73-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08d73-115">Application</span></span>                            | <span data-ttu-id="08d73-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d73-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="08d73-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="08d73-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="08d73-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="08d73-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="08d73-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08d73-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08d73-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08d73-120">Optional query parameters</span></span>

<span data-ttu-id="08d73-121">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="08d73-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="08d73-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="08d73-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="08d73-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08d73-123">Request headers</span></span>

| <span data-ttu-id="08d73-124">Имя</span><span class="sxs-lookup"><span data-stu-id="08d73-124">Name</span></span>      |<span data-ttu-id="08d73-125">Описание</span><span class="sxs-lookup"><span data-stu-id="08d73-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08d73-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08d73-126">Authorization</span></span> | <span data-ttu-id="08d73-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08d73-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08d73-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08d73-129">Request body</span></span>

<span data-ttu-id="08d73-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08d73-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08d73-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="08d73-131">Response</span></span>

<span data-ttu-id="08d73-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенные объекты [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08d73-132">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08d73-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="08d73-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08d73-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="08d73-134">Request</span></span>

<span data-ttu-id="08d73-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08d73-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests
```
---


### <a name="response"></a><span data-ttu-id="08d73-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="08d73-136">Response</span></span>

<span data-ttu-id="08d73-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08d73-137">The following is an example of the response.</span></span>

> <span data-ttu-id="08d73-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08d73-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientActionMessage": "recipientActionMessage-value",
  "recipientActionDateTime": "datetime-value",
  "senderShiftId": "senderShiftId-value",
  "recipientUserId": "recipientUserId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
