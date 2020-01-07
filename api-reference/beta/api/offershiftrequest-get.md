---
title: Получение Оффершифтрекуест
description: Получение свойств и связей объекта Оффершифтрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 48fa2dc104dc609192232a4f173b314134829fb5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952155"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="828cc-103">Получение Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="828cc-103">Get offerShiftRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="828cc-104">Получение свойств и связей объекта [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="828cc-104">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="828cc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="828cc-105">Permissions</span></span>

<span data-ttu-id="828cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="828cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="828cc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="828cc-108">Permission type</span></span>                        | <span data-ttu-id="828cc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="828cc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="828cc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="828cc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="828cc-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="828cc-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="828cc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="828cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="828cc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="828cc-113">Not supported.</span></span> |
| <span data-ttu-id="828cc-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="828cc-114">Application</span></span>                            | <span data-ttu-id="828cc-115">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="828cc-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="828cc-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="828cc-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="828cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="828cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="828cc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="828cc-118">Optional query parameters</span></span>

<span data-ttu-id="828cc-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="828cc-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="828cc-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="828cc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="828cc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="828cc-121">Request headers</span></span>

| <span data-ttu-id="828cc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="828cc-122">Name</span></span>      |<span data-ttu-id="828cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="828cc-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="828cc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="828cc-124">Authorization</span></span> | <span data-ttu-id="828cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="828cc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="828cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="828cc-127">Request body</span></span>

<span data-ttu-id="828cc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="828cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="828cc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="828cc-129">Response</span></span>

<span data-ttu-id="828cc-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="828cc-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="828cc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="828cc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="828cc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="828cc-132">Request</span></span>

<span data-ttu-id="828cc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="828cc-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests
```

### <a name="response"></a><span data-ttu-id="828cc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="828cc-134">Response</span></span>

<span data-ttu-id="828cc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="828cc-135">The following is an example of the response.</span></span>

> <span data-ttu-id="828cc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="828cc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
