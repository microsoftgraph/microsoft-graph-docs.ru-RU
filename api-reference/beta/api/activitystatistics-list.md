---
title: Список Активитистатистикс
description: Получение коллекции объектов Активитистатистикс.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: db4722b3bb4e648d276c2e4e9b642d68a1caa5a9
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "37723774"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="82ebc-103">Список Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="82ebc-103">List activityStatistics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82ebc-104">Получение коллекции [активитистатистикс](../resources/activitystatistics.md) для пользователя за последнюю полную неделю.</span><span class="sxs-lookup"><span data-stu-id="82ebc-104">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="82ebc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82ebc-105">Permissions</span></span>

<span data-ttu-id="82ebc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82ebc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82ebc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82ebc-108">Permission type</span></span>                        | <span data-ttu-id="82ebc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82ebc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="82ebc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82ebc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="82ebc-111">Analytics.Read</span><span class="sxs-lookup"><span data-stu-id="82ebc-111">Analytics.Read</span></span> |
| <span data-ttu-id="82ebc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82ebc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82ebc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82ebc-113">Not supported.</span></span> |
| <span data-ttu-id="82ebc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82ebc-114">Application</span></span>                            | <span data-ttu-id="82ebc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82ebc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82ebc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82ebc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/analytics/activitystatistics 
GET /users/{id|userPrincipalName}/analytics/activitystatistics/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82ebc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82ebc-117">Optional query parameters</span></span>

<span data-ttu-id="82ebc-118">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="82ebc-118">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82ebc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82ebc-119">Request headers</span></span>

| <span data-ttu-id="82ebc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="82ebc-120">Name</span></span>      |<span data-ttu-id="82ebc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="82ebc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82ebc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82ebc-122">Authorization</span></span> | <span data-ttu-id="82ebc-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="82ebc-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="82ebc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82ebc-124">Request body</span></span>

<span data-ttu-id="82ebc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82ebc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82ebc-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="82ebc-126">Response</span></span>

<span data-ttu-id="82ebc-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [активитистатистикс](../resources/activitystatistics.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82ebc-127">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82ebc-128">Пример</span><span class="sxs-lookup"><span data-stu-id="82ebc-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="82ebc-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="82ebc-129">Request</span></span>

<span data-ttu-id="82ebc-130">Ниже приведен пример запроса статистики всех связанных действий для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="82ebc-130">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="82ebc-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="82ebc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82ebc-132">C#</span><span class="sxs-lookup"><span data-stu-id="82ebc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82ebc-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82ebc-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82ebc-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82ebc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82ebc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="82ebc-135">Response</span></span>

<span data-ttu-id="82ebc-136">Ниже приведен пример ответа со всеми связанными сведениями о действиях для пользователя.</span><span class="sxs-lookup"><span data-stu-id="82ebc-136">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="82ebc-137">Этот отклик показывает только первый день действий недели, чтобы уменьшить его для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="82ebc-137">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="82ebc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82ebc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
