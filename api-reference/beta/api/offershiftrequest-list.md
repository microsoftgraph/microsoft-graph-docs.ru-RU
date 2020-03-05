---
title: Список Оффершифтрекуест
description: Получение свойств и связей всех объектов Оффершифтрекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8722d4f64979e1b899df6d96d56d47baf07db522
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456595"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="284cc-103">Список Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="284cc-103">List offerShiftRequest</span></span>

<span data-ttu-id="284cc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="284cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="284cc-105">Получение свойств и связей всех объектов [оффершифтрекуест](../resources/offershiftrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="284cc-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="284cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="284cc-106">Permissions</span></span>

<span data-ttu-id="284cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="284cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="284cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="284cc-109">Permission type</span></span>                        | <span data-ttu-id="284cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="284cc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="284cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="284cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="284cc-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="284cc-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="284cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="284cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="284cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="284cc-114">Not supported.</span></span> |
| <span data-ttu-id="284cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="284cc-115">Application</span></span>                            | <span data-ttu-id="284cc-116">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="284cc-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="284cc-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="284cc-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="284cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="284cc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="284cc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="284cc-119">Optional query parameters</span></span>

<span data-ttu-id="284cc-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="284cc-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="284cc-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="284cc-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="284cc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="284cc-122">Request headers</span></span>

| <span data-ttu-id="284cc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="284cc-123">Name</span></span>      |<span data-ttu-id="284cc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="284cc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="284cc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="284cc-125">Authorization</span></span> | <span data-ttu-id="284cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="284cc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="284cc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="284cc-128">Request body</span></span>

<span data-ttu-id="284cc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="284cc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="284cc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="284cc-130">Response</span></span>

<span data-ttu-id="284cc-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="284cc-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="284cc-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="284cc-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="284cc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="284cc-133">Request</span></span>

<span data-ttu-id="284cc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="284cc-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="284cc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="284cc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="284cc-136">C#</span><span class="sxs-lookup"><span data-stu-id="284cc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="284cc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="284cc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="284cc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="284cc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="284cc-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="284cc-139">Response</span></span>

<span data-ttu-id="284cc-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="284cc-140">The following is an example of the response.</span></span>

> <span data-ttu-id="284cc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="284cc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
