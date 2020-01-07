---
title: Создание Оффершифтрекуест
description: Создайте экземпляр объекта Оффершифтрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3c7eeb1fbe68e41465b5a55150e72c694dad059d
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952127"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="25532-103">Создание Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="25532-103">Create offerShiftRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25532-104">Создайте экземпляр объекта [оффершифтрекуест](../resources/offershiftrequest.md).</span><span class="sxs-lookup"><span data-stu-id="25532-104">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="25532-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25532-105">Permissions</span></span>

<span data-ttu-id="25532-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25532-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25532-108">Permission type</span></span>                        | <span data-ttu-id="25532-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25532-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="25532-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25532-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="25532-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25532-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="25532-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25532-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25532-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25532-113">Not supported.</span></span> |
| <span data-ttu-id="25532-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="25532-114">Application</span></span>                            | <span data-ttu-id="25532-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="25532-115">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="25532-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="25532-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="25532-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25532-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25532-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="25532-118">Optional query parameters</span></span>

<span data-ttu-id="25532-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="25532-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="25532-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="25532-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="25532-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25532-121">Request headers</span></span>

| <span data-ttu-id="25532-122">Имя</span><span class="sxs-lookup"><span data-stu-id="25532-122">Name</span></span>      |<span data-ttu-id="25532-123">Описание</span><span class="sxs-lookup"><span data-stu-id="25532-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="25532-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25532-124">Authorization</span></span> | <span data-ttu-id="25532-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25532-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25532-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25532-127">Request body</span></span>
<span data-ttu-id="25532-128">Укажите новый объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25532-128">Provide the new [offershiftrequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25532-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="25532-129">Response</span></span>

<span data-ttu-id="25532-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25532-130">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25532-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="25532-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25532-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="25532-132">Request</span></span>

<span data-ttu-id="25532-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25532-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/offershiftrequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c"
}
```

### <a name="response"></a><span data-ttu-id="25532-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="25532-134">Response</span></span>

<span data-ttu-id="25532-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25532-135">The following is an example of the response.</span></span>

> <span data-ttu-id="25532-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25532-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.etag": "\"4000ee23-0000-0700-0000-5d1415f60000\"",
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "createdDateTime": "2019-09-27T01:01:04.566Z",
  "lastModifiedDateTime": "2019-09-28T01:03:48.874Z",
  "assignedTo": "recipient",
  "state": "pending",
  "senderDateTime": "2019-09-27T01:01:04.566",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "senderUserId": "a4704dd0-3f4c-4f2c-9bb5-8cc575703f30",
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "managerUserId": null,
  "recipientActionDateTime": null,
  "recipientActionMessage": null,
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
      "displayName": "Employee 1"
    }
  }
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
