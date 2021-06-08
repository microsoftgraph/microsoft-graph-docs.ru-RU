---
title: 'timeCard: endBreak'
description: Завершение открытого перерыва в определенной карточке времени.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f88697261aae32e978e4910c8d112d55c7ceb5ab
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787918"
---
# <a name="timecard-endbreak"></a><span data-ttu-id="8a32f-103">timeCard: endBreak</span><span class="sxs-lookup"><span data-stu-id="8a32f-103">timeCard: endBreak</span></span>

<span data-ttu-id="8a32f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a32f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a32f-105">Завершение открытого перерыва в определенной [карточке timeCard.](../resources/timeCard.md)</span><span class="sxs-lookup"><span data-stu-id="8a32f-105">End the open break in a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a32f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a32f-106">Permissions</span></span>

<span data-ttu-id="8a32f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a32f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a32f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a32f-109">Permission type</span></span>      | <span data-ttu-id="8a32f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a32f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a32f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a32f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8a32f-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a32f-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a32f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a32f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a32f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a32f-114">Not supported.</span></span>    |
|<span data-ttu-id="8a32f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8a32f-115">Application</span></span> | <span data-ttu-id="8a32f-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="8a32f-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="8a32f-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="8a32f-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a32f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a32f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/endBreak
```

## <a name="request-headers"></a><span data-ttu-id="8a32f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a32f-119">Request headers</span></span>

| <span data-ttu-id="8a32f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a32f-120">Header</span></span>       | <span data-ttu-id="8a32f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8a32f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a32f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a32f-122">Authorization</span></span>  | <span data-ttu-id="8a32f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a32f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8a32f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a32f-125">Content-type</span></span> | <span data-ttu-id="8a32f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a32f-p103">application/json. Required.</span></span>|
| <span data-ttu-id="8a32f-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="8a32f-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="8a32f-129">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="8a32f-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="8a32f-130">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="8a32f-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a32f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a32f-131">Request body</span></span>

<span data-ttu-id="8a32f-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8a32f-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8a32f-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="8a32f-133">Parameter</span></span>    | <span data-ttu-id="8a32f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="8a32f-134">Type</span></span>        | <span data-ttu-id="8a32f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="8a32f-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a32f-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="8a32f-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="8a32f-137">Указать, происходит ли это действие в утвержденной локации.</span><span class="sxs-lookup"><span data-stu-id="8a32f-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="8a32f-138">notes</span><span class="sxs-lookup"><span data-stu-id="8a32f-138">notes</span></span>| [<span data-ttu-id="8a32f-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="8a32f-139">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="8a32f-140">Заметки в конце перерыва.</span><span class="sxs-lookup"><span data-stu-id="8a32f-140">Notes during end of break.</span></span>|

## <a name="response"></a><span data-ttu-id="8a32f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a32f-141">Response</span></span>

<span data-ttu-id="8a32f-142">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8a32f-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8a32f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="8a32f-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a32f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a32f-144">Request</span></span>
<span data-ttu-id="8a32f-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a32f-145">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-endbreak"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/endbreak

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "end break smaple notes"
    }
}
```

### <a name="response"></a><span data-ttu-id="8a32f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a32f-146">Response</span></span>

<span data-ttu-id="8a32f-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8a32f-147">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "End Break",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
