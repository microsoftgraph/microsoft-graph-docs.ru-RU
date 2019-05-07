---
title: 'Call: Субскрибетотоне'
description: Подпишитесь на DTMF (многочастотный многочастотный сигнал). Это позволяет получать уведомления, когда пользователь нажимает клавиши на телефоне "тонального".
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a91f3a3db0a020c45966cdca069495650784742a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635962"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="943dc-104">Call: Субскрибетотоне</span><span class="sxs-lookup"><span data-stu-id="943dc-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="943dc-105">Подпишитесь на DTMF (многочастотный многочастотный сигнал).</span><span class="sxs-lookup"><span data-stu-id="943dc-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="943dc-106">Это позволяет получать уведомления, когда пользователь нажимает клавиши на "тональном" телефоне.</span><span class="sxs-lookup"><span data-stu-id="943dc-106">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="943dc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="943dc-107">Permissions</span></span>
<span data-ttu-id="943dc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="943dc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="943dc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="943dc-110">Permission type</span></span> | <span data-ttu-id="943dc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="943dc-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="943dc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="943dc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="943dc-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="943dc-113">Not Supported</span></span>        |
| <span data-ttu-id="943dc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="943dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="943dc-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="943dc-115">Not Supported</span></span>        |
| <span data-ttu-id="943dc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="943dc-116">Application</span></span>     | <span data-ttu-id="943dc-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="943dc-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="943dc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="943dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="943dc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="943dc-119">Request headers</span></span>
| <span data-ttu-id="943dc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="943dc-120">Name</span></span>          | <span data-ttu-id="943dc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="943dc-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="943dc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="943dc-122">Authorization</span></span> | <span data-ttu-id="943dc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="943dc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="943dc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="943dc-125">Request body</span></span>
<span data-ttu-id="943dc-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="943dc-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="943dc-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="943dc-127">Parameter</span></span>      | <span data-ttu-id="943dc-128">Тип</span><span class="sxs-lookup"><span data-stu-id="943dc-128">Type</span></span>    | <span data-ttu-id="943dc-129">Описание</span><span class="sxs-lookup"><span data-stu-id="943dc-129">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="943dc-130">Контекст</span><span class="sxs-lookup"><span data-stu-id="943dc-130">clientContext</span></span>  | <span data-ttu-id="943dc-131">String</span><span class="sxs-lookup"><span data-stu-id="943dc-131">String</span></span>  | <span data-ttu-id="943dc-132">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="943dc-132">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="943dc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="943dc-133">Response</span></span>
<span data-ttu-id="943dc-134">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="943dc-134">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="943dc-135">Пример</span><span class="sxs-lookup"><span data-stu-id="943dc-135">Example</span></span>
<span data-ttu-id="943dc-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="943dc-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="943dc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="943dc-137">Request</span></span>
<span data-ttu-id="943dc-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="943dc-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="943dc-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="943dc-139">Response</span></span>

> <span data-ttu-id="943dc-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="943dc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="943dc-142">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="943dc-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="943dc-143">Языках</span><span class="sxs-lookup"><span data-stu-id="943dc-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-subscribeToTone-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="943dc-144">Язык</span><span class="sxs-lookup"><span data-stu-id="943dc-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-subscribeToTone-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---operation-completed"></a><span data-ttu-id="943dc-145">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="943dc-145">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-subscribetotone.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-subscribetotone.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
