---
title: 'timeCard: startBreak'
description: Начните перерыв в определенной карточке времени.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 95c220d9b6bcead0f0c734959bb99788e8b5e2fd
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787895"
---
# <a name="timecard-startbreak"></a><span data-ttu-id="b4a19-103">timeCard: startBreak</span><span class="sxs-lookup"><span data-stu-id="b4a19-103">timeCard: startBreak</span></span>

<span data-ttu-id="b4a19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4a19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4a19-105">Начните перерыв в определенной [timeCard](../resources/timeCard.md).</span><span class="sxs-lookup"><span data-stu-id="b4a19-105">Start a break in a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4a19-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a19-106">Permissions</span></span>

<span data-ttu-id="b4a19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4a19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4a19-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a19-109">Permission type</span></span>      | <span data-ttu-id="b4a19-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4a19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4a19-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4a19-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b4a19-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4a19-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4a19-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4a19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4a19-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a19-114">Not supported.</span></span>    |
|<span data-ttu-id="b4a19-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b4a19-115">Application</span></span> | <span data-ttu-id="b4a19-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="b4a19-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="b4a19-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="b4a19-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="b4a19-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4a19-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/startBreak
```

## <a name="request-headers"></a><span data-ttu-id="b4a19-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4a19-119">Request headers</span></span>

| <span data-ttu-id="b4a19-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4a19-120">Header</span></span>       | <span data-ttu-id="b4a19-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b4a19-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4a19-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4a19-122">Authorization</span></span>  | <span data-ttu-id="b4a19-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4a19-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b4a19-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4a19-125">Content-type</span></span> | <span data-ttu-id="b4a19-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4a19-p103">application/json. Required.</span></span>|
| <span data-ttu-id="b4a19-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="b4a19-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="b4a19-129">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="b4a19-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="b4a19-130">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="b4a19-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4a19-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4a19-131">Request body</span></span>

<span data-ttu-id="b4a19-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b4a19-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b4a19-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="b4a19-133">Parameter</span></span>    | <span data-ttu-id="b4a19-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b4a19-134">Type</span></span>        | <span data-ttu-id="b4a19-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b4a19-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4a19-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="b4a19-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="b4a19-137">Указать, происходит ли это действие в утвержденной локации.</span><span class="sxs-lookup"><span data-stu-id="b4a19-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="b4a19-138">notes</span><span class="sxs-lookup"><span data-stu-id="b4a19-138">notes</span></span>| [<span data-ttu-id="b4a19-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="b4a19-139">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="b4a19-140">Заметки во время начала перерыва.</span><span class="sxs-lookup"><span data-stu-id="b4a19-140">Notes during start of break.</span></span>|

## <a name="response"></a><span data-ttu-id="b4a19-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a19-141">Response</span></span>

<span data-ttu-id="b4a19-142">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4a19-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4a19-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b4a19-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4a19-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4a19-144">Request</span></span>
<span data-ttu-id="b4a19-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4a19-145">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-startBreak"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/startbreak
Content-type: application/json

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "start break smaple notes"
    }
}
```

### <a name="response"></a><span data-ttu-id="b4a19-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a19-146">Response</span></span>

<span data-ttu-id="b4a19-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4a19-147">The following is an example of the response.</span></span> 

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
  "description": "Start Break",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
