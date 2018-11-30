---
title: 'вызов: subscribeToTone'
description: " Телефон."
ms.openlocfilehash: c3793931c2f06e54cdac278f0f0539b42d7e622c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079355"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="48280-103">вызов: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="48280-103">call: subscribeToTone</span></span>

> <span data-ttu-id="48280-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48280-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48280-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48280-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48280-106">Подпишитесь на DTMF (двухтональный несколькими частота сигналы).</span><span class="sxs-lookup"><span data-stu-id="48280-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="48280-107">Это позволяет получать уведомления при нажатии клавиш на телефоне «тонального сигнала».</span><span class="sxs-lookup"><span data-stu-id="48280-107">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="48280-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48280-108">Permissions</span></span>
<span data-ttu-id="48280-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48280-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48280-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48280-111">Permission type</span></span> | <span data-ttu-id="48280-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48280-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="48280-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48280-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="48280-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="48280-114">Not Supported</span></span>        |
| <span data-ttu-id="48280-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48280-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48280-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="48280-116">Not Supported</span></span>        |
| <span data-ttu-id="48280-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="48280-117">Application</span></span>     | <span data-ttu-id="48280-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="48280-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="48280-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48280-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="48280-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48280-120">Request headers</span></span>
| <span data-ttu-id="48280-121">Имя</span><span class="sxs-lookup"><span data-stu-id="48280-121">Name</span></span>          | <span data-ttu-id="48280-122">Описание</span><span class="sxs-lookup"><span data-stu-id="48280-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="48280-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48280-123">Authorization</span></span> | <span data-ttu-id="48280-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48280-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48280-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48280-126">Request body</span></span>
<span data-ttu-id="48280-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="48280-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="48280-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="48280-128">Parameter</span></span>      | <span data-ttu-id="48280-129">Тип</span><span class="sxs-lookup"><span data-stu-id="48280-129">Type</span></span>    | <span data-ttu-id="48280-130">Description</span><span class="sxs-lookup"><span data-stu-id="48280-130">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="48280-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="48280-131">clientContext</span></span>  | <span data-ttu-id="48280-132">String</span><span class="sxs-lookup"><span data-stu-id="48280-132">String</span></span>  | <span data-ttu-id="48280-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="48280-133">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="48280-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="48280-134">Response</span></span>
<span data-ttu-id="48280-135">Возвращает `202 Accepted` код ответа и расположения заголовком с uri для [commsOperation](../resources/commsoperation.md) , созданные для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="48280-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="48280-136">Пример</span><span class="sxs-lookup"><span data-stu-id="48280-136">Example</span></span>
<span data-ttu-id="48280-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="48280-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="48280-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="48280-138">Request</span></span>
<span data-ttu-id="48280-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48280-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="48280-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="48280-140">Response</span></span>

> <span data-ttu-id="48280-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48280-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="48280-143">Уведомления - операция завершена</span><span class="sxs-lookup"><span data-stu-id="48280-143">Notification - operation completed</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
