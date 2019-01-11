---
title: Создание объекта event
description: С помощью этого API можно создать событие.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 4b7e0803b6eb59a2446da658815c19d08256587b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883911"
---
# <a name="create-event"></a><span data-ttu-id="1e13c-103">Создание объекта event</span><span class="sxs-lookup"><span data-stu-id="1e13c-103">Create event</span></span>

> <span data-ttu-id="1e13c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1e13c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e13c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e13c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e13c-106">С помощью этого API можно создать [событие](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1e13c-106">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e13c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e13c-107">Permissions</span></span>
<span data-ttu-id="1e13c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e13c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e13c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e13c-110">Permission type</span></span>      | <span data-ttu-id="1e13c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e13c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e13c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e13c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e13c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e13c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1e13c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e13c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e13c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e13c-115">Not supported.</span></span>    |
|<span data-ttu-id="1e13c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e13c-116">Application</span></span> | <span data-ttu-id="1e13c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e13c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e13c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e13c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="1e13c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e13c-119">Request headers</span></span>
| <span data-ttu-id="1e13c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e13c-120">Header</span></span>       | <span data-ttu-id="1e13c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1e13c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e13c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e13c-122">Authorization</span></span>  | <span data-ttu-id="1e13c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e13c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e13c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e13c-125">Request body</span></span>
<span data-ttu-id="1e13c-126">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e13c-126">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1e13c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e13c-127">Response</span></span>
<span data-ttu-id="1e13c-128">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1e13c-128">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e13c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1e13c-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1e13c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e13c-130">Request</span></span>
<span data-ttu-id="1e13c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e13c-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="1e13c-132">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e13c-132">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="1e13c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e13c-133">Response</span></span>
<span data-ttu-id="1e13c-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1e13c-134">The following is an example of the response.</span></span>
><span data-ttu-id="1e13c-135">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="1e13c-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1e13c-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e13c-136">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
