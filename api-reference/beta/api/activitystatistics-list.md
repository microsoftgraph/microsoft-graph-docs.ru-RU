---
title: Список Активитистатистикс
description: Получение коллекции объектов Активитистатистикс.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: ba1fb1fb18b3791b43d17ffeb11fadf7edd608aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952508"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="75344-103">Список Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="75344-103">List activityStatistics</span></span>

<span data-ttu-id="75344-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75344-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75344-105">Получение коллекции [активитистатистикс](../resources/activitystatistics.md) для пользователя за последнюю полную неделю.</span><span class="sxs-lookup"><span data-stu-id="75344-105">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="75344-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75344-106">Permissions</span></span>

<span data-ttu-id="75344-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75344-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75344-109">Permission type</span></span>                        | <span data-ttu-id="75344-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75344-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="75344-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75344-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="75344-112">Analytics.Read</span><span class="sxs-lookup"><span data-stu-id="75344-112">Analytics.Read</span></span> |
| <span data-ttu-id="75344-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75344-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75344-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75344-114">Not supported.</span></span> |
| <span data-ttu-id="75344-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75344-115">Application</span></span>                            | <span data-ttu-id="75344-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75344-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75344-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75344-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/analytics/activitystatistics
GET /users/{id|userPrincipalName}/analytics/activitystatistics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75344-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75344-118">Optional query parameters</span></span>

<span data-ttu-id="75344-119">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="75344-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75344-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75344-120">Request headers</span></span>

| <span data-ttu-id="75344-121">Имя</span><span class="sxs-lookup"><span data-stu-id="75344-121">Name</span></span>      |<span data-ttu-id="75344-122">Описание</span><span class="sxs-lookup"><span data-stu-id="75344-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75344-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75344-123">Authorization</span></span> | <span data-ttu-id="75344-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="75344-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="75344-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75344-125">Request body</span></span>

<span data-ttu-id="75344-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75344-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75344-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="75344-127">Response</span></span>

<span data-ttu-id="75344-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [активитистатистикс](../resources/activitystatistics.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75344-128">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75344-129">Пример</span><span class="sxs-lookup"><span data-stu-id="75344-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="75344-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="75344-130">Request</span></span>

<span data-ttu-id="75344-131">Ниже приведен пример запроса статистики всех связанных действий для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="75344-131">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="75344-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="75344-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```
# <a name="c"></a>[<span data-ttu-id="75344-133">C#</span><span class="sxs-lookup"><span data-stu-id="75344-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75344-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75344-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75344-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75344-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75344-136">Java</span><span class="sxs-lookup"><span data-stu-id="75344-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitystatistics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75344-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="75344-137">Response</span></span>

<span data-ttu-id="75344-138">Ниже приведен пример ответа со всеми связанными сведениями о действиях для пользователя.</span><span class="sxs-lookup"><span data-stu-id="75344-138">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="75344-139">Этот отклик показывает только первый день действий недели, чтобы уменьшить его для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75344-139">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="75344-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75344-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityStatistics",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#activitystatistics",
    "value": [
        {
            "@odata.type": "#microsoft.graph.emailActivityStatistics",
            "activity": "Email",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "email_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S",
            "readEmail": "PT0S",
            "sentEmail": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.meetingActivityStatistics",
            "activity": "Meeting",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "meeting_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S",
            "organized": "PT0S",
            "recurring": "PT0S",
            "long": "PT0S",
            "conflicting": "PT0S",
            "multitasking": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.focusActivityStatistics",
            "activity": "Focus",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "focus_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.chatActivityStatistics",
            "activity": "Chat",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "chat_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.callActivityStatistics",
            "activity": "Call",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "call_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List activitystatistics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


