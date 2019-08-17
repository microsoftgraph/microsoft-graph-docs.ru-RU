---
title: Список Активитистатистикс
description: Получение коллекции объектов Активитистатистикс.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 683dacd86088b2d306abbc36a15e890edbdc1ae6
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450797"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="7f915-103">Список Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="7f915-103">List activityStatistics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f915-104">Получение коллекции [активитистатистикс](../resources/activitystatistics.md) для пользователя за последнюю полную неделю.</span><span class="sxs-lookup"><span data-stu-id="7f915-104">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f915-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f915-105">Permissions</span></span>

<span data-ttu-id="7f915-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f915-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f915-108">Permission type</span></span>                        | <span data-ttu-id="7f915-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f915-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7f915-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f915-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f915-111">Analytics. Read</span><span class="sxs-lookup"><span data-stu-id="7f915-111">Analytics.Read</span></span> |
| <span data-ttu-id="7f915-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f915-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f915-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f915-113">Not supported.</span></span> |
| <span data-ttu-id="7f915-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f915-114">Application</span></span>                            | <span data-ttu-id="7f915-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f915-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f915-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f915-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET  https://graph.microsoft.com/beta/me/analytics/activitystatistics 
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/analytics/activitystatistics/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f915-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f915-117">Optional query parameters</span></span>

<span data-ttu-id="7f915-118">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7f915-118">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f915-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f915-119">Request headers</span></span>

| <span data-ttu-id="7f915-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7f915-120">Name</span></span>      |<span data-ttu-id="7f915-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7f915-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f915-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f915-122">Authorization</span></span> | <span data-ttu-id="7f915-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="7f915-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f915-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f915-124">Request body</span></span>

<span data-ttu-id="7f915-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f915-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f915-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f915-126">Response</span></span>

<span data-ttu-id="7f915-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [активитистатистикс](../resources/activitystatistics.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f915-127">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f915-128">Пример</span><span class="sxs-lookup"><span data-stu-id="7f915-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f915-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f915-129">Request</span></span>

<span data-ttu-id="7f915-130">Ниже приведен пример запроса статистики всех связанных действий для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="7f915-130">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```

### <a name="response"></a><span data-ttu-id="7f915-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f915-131">Response</span></span>

<span data-ttu-id="7f915-132">Ниже приведен пример ответа со всеми связанными сведениями о действиях для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7f915-132">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="7f915-133">Этот отклик показывает только первый день действий недели, чтобы уменьшить его для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7f915-133">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="7f915-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f915-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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