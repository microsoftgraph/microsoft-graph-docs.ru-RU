---
title: Создание объекта event
description: С помощью этого API можно создать событие.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 193cb6214d807c329d135f026f239bd6a36c236e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529812"
---
# <a name="create-event"></a><span data-ttu-id="fbeec-103">Создание объекта event</span><span class="sxs-lookup"><span data-stu-id="fbeec-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbeec-104">С помощью этого API можно создать [событие](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="fbeec-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbeec-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbeec-105">Permissions</span></span>
<span data-ttu-id="fbeec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbeec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbeec-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbeec-108">Permission type</span></span>      | <span data-ttu-id="fbeec-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbeec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbeec-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbeec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fbeec-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbeec-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fbeec-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbeec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbeec-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbeec-113">Not supported.</span></span>    |
|<span data-ttu-id="fbeec-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbeec-114">Application</span></span> | <span data-ttu-id="fbeec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbeec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbeec-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbeec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="fbeec-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbeec-117">Request headers</span></span>
| <span data-ttu-id="fbeec-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbeec-118">Header</span></span>       | <span data-ttu-id="fbeec-119">Значение</span><span class="sxs-lookup"><span data-stu-id="fbeec-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbeec-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbeec-120">Authorization</span></span>  | <span data-ttu-id="fbeec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbeec-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbeec-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbeec-123">Request body</span></span>
<span data-ttu-id="fbeec-124">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbeec-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fbeec-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbeec-125">Response</span></span>
<span data-ttu-id="fbeec-126">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fbeec-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbeec-127">Пример</span><span class="sxs-lookup"><span data-stu-id="fbeec-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fbeec-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbeec-128">Request</span></span>
<span data-ttu-id="fbeec-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbeec-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="fbeec-130">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbeec-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="fbeec-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbeec-131">Response</span></span>
<span data-ttu-id="fbeec-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fbeec-132">The following is an example of the response.</span></span>
><span data-ttu-id="fbeec-133">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fbeec-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fbeec-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbeec-134">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
