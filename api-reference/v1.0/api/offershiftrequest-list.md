---
title: Список Оффершифтрекуест
description: Получение свойств и связей всех объектов Оффершифтрекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a0cba82f3a96da35b18b5e11094aac72706b384
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217268"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="cc5e5-103">Список Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="cc5e5-103">List offerShiftRequest</span></span>

<span data-ttu-id="cc5e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc5e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc5e5-105">Получение свойств и связей всех объектов [оффершифтрекуест](../resources/offershiftrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc5e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc5e5-106">Permissions</span></span>

<span data-ttu-id="cc5e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc5e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc5e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc5e5-109">Permission type</span></span>                        | <span data-ttu-id="cc5e5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc5e5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cc5e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc5e5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc5e5-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cc5e5-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cc5e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc5e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc5e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-114">Not supported.</span></span> |
| <span data-ttu-id="cc5e5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc5e5-115">Application</span></span>                            | <span data-ttu-id="cc5e5-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc5e5-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="cc5e5-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cc5e5-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cc5e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc5e5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc5e5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc5e5-120">Optional query parameters</span></span>

<span data-ttu-id="cc5e5-121">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cc5e5-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cc5e5-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc5e5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc5e5-123">Request headers</span></span>

| <span data-ttu-id="cc5e5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="cc5e5-124">Name</span></span>      |<span data-ttu-id="cc5e5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="cc5e5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cc5e5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc5e5-126">Authorization</span></span> | <span data-ttu-id="cc5e5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc5e5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc5e5-129">Request body</span></span>

<span data-ttu-id="cc5e5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc5e5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc5e5-131">Response</span></span>

<span data-ttu-id="cc5e5-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенные объекты [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-132">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc5e5-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc5e5-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc5e5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc5e5-134">Request</span></span>

<span data-ttu-id="cc5e5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc5e5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc5e5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="cc5e5-137">C#</span><span class="sxs-lookup"><span data-stu-id="cc5e5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc5e5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc5e5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc5e5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc5e5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc5e5-140">Java</span><span class="sxs-lookup"><span data-stu-id="cc5e5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="cc5e5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc5e5-141">Response</span></span>

<span data-ttu-id="cc5e5-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-142">The following is an example of the response.</span></span>

> <span data-ttu-id="cc5e5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc5e5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
