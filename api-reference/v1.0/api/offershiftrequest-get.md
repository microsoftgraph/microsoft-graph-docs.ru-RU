---
title: Получение Оффершифтрекуест
description: Получение свойств и связей объекта Оффершифтрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c997fb52a05a0debb30a89b99736a2ede8abcd19
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154937"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="1b074-103">Получение Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="1b074-103">Get offerShiftRequest</span></span>

<span data-ttu-id="1b074-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b074-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b074-105">Получение свойств и связей объекта [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="1b074-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b074-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b074-106">Permissions</span></span>

<span data-ttu-id="1b074-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b074-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b074-109">Permission type</span></span>                        | <span data-ttu-id="1b074-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b074-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1b074-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b074-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b074-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1b074-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1b074-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b074-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b074-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b074-114">Not supported.</span></span> |
| <span data-ttu-id="1b074-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b074-115">Application</span></span>                            | <span data-ttu-id="1b074-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1b074-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="1b074-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="1b074-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1b074-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="1b074-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1b074-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b074-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b074-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1b074-120">Optional query parameters</span></span>

<span data-ttu-id="1b074-121">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1b074-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b074-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b074-122">Request headers</span></span>

| <span data-ttu-id="1b074-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1b074-123">Name</span></span>      |<span data-ttu-id="1b074-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1b074-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b074-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b074-125">Authorization</span></span> | <span data-ttu-id="1b074-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b074-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b074-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b074-128">Request body</span></span>

<span data-ttu-id="1b074-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b074-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b074-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b074-130">Response</span></span>

<span data-ttu-id="1b074-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b074-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b074-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="1b074-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b074-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b074-133">Request</span></span>

<span data-ttu-id="1b074-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b074-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
---


### <a name="response"></a><span data-ttu-id="1b074-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b074-135">Response</span></span>

<span data-ttu-id="1b074-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1b074-136">The following is an example of the response.</span></span>

> <span data-ttu-id="1b074-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b074-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
