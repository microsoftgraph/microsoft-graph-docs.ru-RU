---
title: List activityStatistics
description: Получите коллекцию объектов activityStatistics.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 422d6b3d03129d2e1c7169f3131c46fadc457e35
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048311"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="32707-103">List activityStatistics</span><span class="sxs-lookup"><span data-stu-id="32707-103">List activityStatistics</span></span>

<span data-ttu-id="32707-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32707-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32707-105">Получите коллекцию [действийStatistics](../resources/activitystatistics.md) для пользователя за последнюю полную неделю.</span><span class="sxs-lookup"><span data-stu-id="32707-105">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="32707-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32707-106">Permissions</span></span>

<span data-ttu-id="32707-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32707-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32707-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32707-109">Permission type</span></span>                        | <span data-ttu-id="32707-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32707-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="32707-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32707-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="32707-112">Analytics.Read</span><span class="sxs-lookup"><span data-stu-id="32707-112">Analytics.Read</span></span> |
| <span data-ttu-id="32707-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32707-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32707-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32707-114">Not supported.</span></span> |
| <span data-ttu-id="32707-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32707-115">Application</span></span>                            | <span data-ttu-id="32707-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32707-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32707-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32707-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/analytics/activitystatistics
GET /users/{id|userPrincipalName}/analytics/activitystatistics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32707-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="32707-118">Optional query parameters</span></span>

<span data-ttu-id="32707-119">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="32707-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32707-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32707-120">Request headers</span></span>

| <span data-ttu-id="32707-121">Имя</span><span class="sxs-lookup"><span data-stu-id="32707-121">Name</span></span>      |<span data-ttu-id="32707-122">Описание</span><span class="sxs-lookup"><span data-stu-id="32707-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="32707-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32707-123">Authorization</span></span> | <span data-ttu-id="32707-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="32707-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="32707-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32707-125">Request body</span></span>

<span data-ttu-id="32707-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32707-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32707-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="32707-127">Response</span></span>

<span data-ttu-id="32707-128">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [activityStatistics](../resources/activitystatistics.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="32707-128">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32707-129">Пример</span><span class="sxs-lookup"><span data-stu-id="32707-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="32707-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="32707-130">Request</span></span>

<span data-ttu-id="32707-131">Ниже приводится пример запроса всей связанной статистики действий для подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="32707-131">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="32707-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="32707-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```
# <a name="c"></a>[<span data-ttu-id="32707-133">C#</span><span class="sxs-lookup"><span data-stu-id="32707-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32707-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32707-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32707-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32707-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32707-136">Java</span><span class="sxs-lookup"><span data-stu-id="32707-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitystatistics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="32707-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="32707-137">Response</span></span>

<span data-ttu-id="32707-138">Ниже приводится пример ответа со всей связанной статистикой действий для пользователя.</span><span class="sxs-lookup"><span data-stu-id="32707-138">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="32707-139">В этом ответе показан только первый день недельных действий, чтобы сократить его для чтения.</span><span class="sxs-lookup"><span data-stu-id="32707-139">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="32707-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="32707-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


