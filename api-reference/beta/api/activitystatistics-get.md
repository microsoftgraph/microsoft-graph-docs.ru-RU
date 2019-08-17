---
title: Получение Активитистатистикс
description: Получение свойств объекта Активитистатистикс для пользователя.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 9a85211faf15b6edbf843c5c604251dae06ae0a3
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450798"
---
# <a name="get-activitystatistics"></a><span data-ttu-id="a738d-103">Получение Активитистатистикс</span><span class="sxs-lookup"><span data-stu-id="a738d-103">Get activityStatistics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a738d-104">Получение свойств объекта [активитистатистикс](../resources/activitystatistics.md) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a738d-104">Get the properties of an [activityStatistics](../resources/activitystatistics.md) object for a user.</span></span>

<span data-ttu-id="a738d-105">Можно получить свойства типа [активитистатистикс](../resources/activitystatistics.md) для указанного пользователя и диапазона дат.</span><span class="sxs-lookup"><span data-stu-id="a738d-105">You can get the properties of a type of [activityStatistics](../resources/activitystatistics.md) for the specified user and date range.</span></span> <span data-ttu-id="a738d-106">Вы можете указать тип статистики и диапазон дат, используя поддерживаемый формат для `id` [свойства идентификатора действия](../resources/activitystatistics.md#activity-id-property) в запросе.</span><span class="sxs-lookup"><span data-stu-id="a738d-106">You can specify the type of statistics and date range by using the supported format of the [activity id property](../resources/activitystatistics.md#activity-id-property) for `id` in the query.</span></span>

## <a name="permissions"></a><span data-ttu-id="a738d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a738d-107">Permissions</span></span>

<span data-ttu-id="a738d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a738d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a738d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a738d-110">Permission type</span></span>                        | <span data-ttu-id="a738d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a738d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a738d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a738d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a738d-113">Analytics. Read</span><span class="sxs-lookup"><span data-stu-id="a738d-113">Analytics.Read</span></span> |
| <span data-ttu-id="a738d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a738d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a738d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a738d-115">Not supported.</span></span> |
| <span data-ttu-id="a738d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a738d-116">Application</span></span>                            | <span data-ttu-id="a738d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a738d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a738d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a738d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" }  -->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/{id}

GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/analytics/activitystatistics/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="a738d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a738d-119">Optional query parameters</span></span>

<span data-ttu-id="a738d-120">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a738d-120">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a738d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a738d-121">Request headers</span></span>

| <span data-ttu-id="a738d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a738d-122">Name</span></span>      |<span data-ttu-id="a738d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a738d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a738d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a738d-124">Authorization</span></span> | <span data-ttu-id="a738d-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a738d-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a738d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a738d-126">Request body</span></span>

<span data-ttu-id="a738d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a738d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a738d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a738d-128">Response</span></span>

<span data-ttu-id="a738d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный тип статистики действий, который является одним из следующих ресурсов, производных от [Активитистатистикс](../resources/activitystatistics.md): {[Call](../resources/callactivitystatistics.md), [Chat](../resources/chatactivitystatistics.md), [Email](../resources/emailactivitystatistics.md), [Focus](../resources/focusactivitystatistics.md), и [собрание](../resources/meetingactivitystatistics.md)}.</span><span class="sxs-lookup"><span data-stu-id="a738d-129">If successful, this method returns a `200 OK` response code and the requested type of activity statistics, which is one of the following resources derived from [activityStatistics](../resources/activitystatistics.md):{[Call](../resources/callactivitystatistics.md), [Chat](../resources/chatactivitystatistics.md), [Email](../resources/emailactivitystatistics.md), [Focus](../resources/focusactivitystatistics.md), and [Meeting](../resources/meetingactivitystatistics.md)}.</span></span>

## <a name="example"></a><span data-ttu-id="a738d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a738d-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a738d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a738d-131">Request</span></span>

<span data-ttu-id="a738d-132">В следующем примере запрашиваются статистические данные о типе Емаилактивитистатистикс пользователя, выполнившего вход в систему, в диапазоне дат от 2019-06-16 до 2019-06-17.</span><span class="sxs-lookup"><span data-stu-id="a738d-132">The following example requests statistics of the type emailActivityStatistics of the signed-in user, for the date range between 2019-06-16 and 2019-06-17.</span></span> <span data-ttu-id="a738d-133">Дополнительные сведения о формате свойства "общий идентификатор" можно узнать в разделе [свойство ID действия](../resources/activitystatistics.md#activity-id-property).</span><span class="sxs-lookup"><span data-stu-id="a738d-133">For more information about the general id property format, see [activity id property](../resources/activitystatistics.md#activity-id-property).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/email_2019-06-16_2019-06-17

```

#### <a name="response"></a><span data-ttu-id="a738d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a738d-134">Response</span></span>

<span data-ttu-id="a738d-135">Ниже приведен пример ответа, который получает статистику действий пользователя, выполнившего вход, для определенного действия и дня.</span><span class="sxs-lookup"><span data-stu-id="a738d-135">The following is an example of the response that gets activity statistics of a signed-in user for a specific activity and day.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityStatistics"
} -->

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#activitystatistics/$entity",
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
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activityStatistics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
