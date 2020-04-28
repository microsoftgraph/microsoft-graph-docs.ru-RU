---
title: Получение Оффершифтрекуест
description: Получение свойств и связей объекта Оффершифтрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c1ae04f4e2cd97cca0ad0f7c7719c4f1b6d4b5c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456593"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="5bcb0-103">Получение Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="5bcb0-103">Get offerShiftRequest</span></span>

<span data-ttu-id="5bcb0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bcb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bcb0-105">Получение свойств и связей объекта [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="5bcb0-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bcb0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bcb0-106">Permissions</span></span>

<span data-ttu-id="5bcb0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bcb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bcb0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bcb0-109">Permission type</span></span>                        | <span data-ttu-id="5bcb0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bcb0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5bcb0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bcb0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bcb0-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bcb0-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5bcb0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bcb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bcb0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bcb0-114">Not supported.</span></span> |
| <span data-ttu-id="5bcb0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bcb0-115">Application</span></span>                            | <span data-ttu-id="5bcb0-116">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="5bcb0-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="5bcb0-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="5bcb0-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="5bcb0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bcb0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bcb0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5bcb0-119">Optional query parameters</span></span>

<span data-ttu-id="5bcb0-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5bcb0-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5bcb0-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5bcb0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bcb0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bcb0-122">Request headers</span></span>

| <span data-ttu-id="5bcb0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5bcb0-123">Name</span></span>      |<span data-ttu-id="5bcb0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5bcb0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5bcb0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bcb0-125">Authorization</span></span> | <span data-ttu-id="5bcb0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bcb0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bcb0-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bcb0-128">Request body</span></span>

<span data-ttu-id="5bcb0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bcb0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bcb0-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5bcb0-130">Response</span></span>

<span data-ttu-id="5bcb0-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5bcb0-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5bcb0-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="5bcb0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5bcb0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bcb0-133">Request</span></span>

<span data-ttu-id="5bcb0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bcb0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5bcb0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bcb0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="5bcb0-136">C#</span><span class="sxs-lookup"><span data-stu-id="5bcb0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bcb0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bcb0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bcb0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bcb0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5bcb0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bcb0-139">Response</span></span>

<span data-ttu-id="5bcb0-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5bcb0-140">The following is an example of the response.</span></span>

> <span data-ttu-id="5bcb0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bcb0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
