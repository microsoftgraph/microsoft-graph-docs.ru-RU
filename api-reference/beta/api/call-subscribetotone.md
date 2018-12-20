---
title: 'вызов: subscribeToTone'
description: Подпишитесь на DTMF (двухтональный несколькими частота сигналы). Это позволяет получать уведомления при нажатии клавиш на телефоне «тонального сигнала».
author: VinodRavichandran
ms.openlocfilehash: 82f7632736dc187fae1313224a6cb6f4807e0dd1
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380438"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="db149-104">вызов: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="db149-104">call: subscribeToTone</span></span>

> <span data-ttu-id="db149-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db149-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db149-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db149-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db149-107">Подпишитесь на DTMF (двухтональный несколькими частота сигналы).</span><span class="sxs-lookup"><span data-stu-id="db149-107">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="db149-108">Это позволяет получать уведомления при нажатии клавиш на телефоне «тонального сигнала».</span><span class="sxs-lookup"><span data-stu-id="db149-108">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="db149-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db149-109">Permissions</span></span>
<span data-ttu-id="db149-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db149-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db149-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db149-112">Permission type</span></span> | <span data-ttu-id="db149-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db149-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="db149-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db149-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="db149-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db149-115">Not Supported</span></span>        |
| <span data-ttu-id="db149-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db149-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db149-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db149-117">Not Supported</span></span>        |
| <span data-ttu-id="db149-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db149-118">Application</span></span>     | <span data-ttu-id="db149-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="db149-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="db149-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db149-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="db149-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db149-121">Request headers</span></span>
| <span data-ttu-id="db149-122">Имя</span><span class="sxs-lookup"><span data-stu-id="db149-122">Name</span></span>          | <span data-ttu-id="db149-123">Описание</span><span class="sxs-lookup"><span data-stu-id="db149-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="db149-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db149-124">Authorization</span></span> | <span data-ttu-id="db149-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db149-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db149-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db149-127">Request body</span></span>
<span data-ttu-id="db149-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="db149-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="db149-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="db149-129">Parameter</span></span>      | <span data-ttu-id="db149-130">Тип</span><span class="sxs-lookup"><span data-stu-id="db149-130">Type</span></span>    | <span data-ttu-id="db149-131">Описание</span><span class="sxs-lookup"><span data-stu-id="db149-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="db149-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="db149-132">clientContext</span></span>  | <span data-ttu-id="db149-133">String</span><span class="sxs-lookup"><span data-stu-id="db149-133">String</span></span>  | <span data-ttu-id="db149-134">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="db149-134">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="db149-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="db149-135">Response</span></span>
<span data-ttu-id="db149-136">Возвращает `202 Accepted` код ответа и расположения заголовком с uri для [commsOperation](../resources/commsoperation.md) , созданные для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="db149-136">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="db149-137">Пример</span><span class="sxs-lookup"><span data-stu-id="db149-137">Example</span></span>
<span data-ttu-id="db149-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="db149-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="db149-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="db149-139">Request</span></span>
<span data-ttu-id="db149-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db149-140">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="db149-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="db149-141">Response</span></span>

> <span data-ttu-id="db149-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db149-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="db149-144">Уведомления - операция завершена</span><span class="sxs-lookup"><span data-stu-id="db149-144">Notification - operation completed</span></span>

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
