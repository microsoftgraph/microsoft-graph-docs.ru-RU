---
title: 'Call: Субскрибетотоне'
description: Подпишитесь на DTMF (многочастотный многочастотный сигнал). Это позволяет получать уведомления, когда пользователь нажимает клавиши в "Диалпад".
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 83e6c1b9795ea1caf27a166fd523c70b51909df0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418868"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="a6e7f-104">Call: Субскрибетотоне</span><span class="sxs-lookup"><span data-stu-id="a6e7f-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6e7f-105">Подпишитесь на DTMF (многочастотный многочастотный сигнал).</span><span class="sxs-lookup"><span data-stu-id="a6e7f-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="a6e7f-106">Это позволяет получать уведомления, когда пользователь нажимает клавиши в "Диалпад".</span><span class="sxs-lookup"><span data-stu-id="a6e7f-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="a6e7f-107">Действие **субскрибетотоне** поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="a6e7f-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6e7f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6e7f-108">Permissions</span></span>
<span data-ttu-id="a6e7f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6e7f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6e7f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6e7f-111">Permission type</span></span> | <span data-ttu-id="a6e7f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6e7f-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="a6e7f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6e7f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6e7f-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a6e7f-114">Not Supported</span></span>        |
| <span data-ttu-id="a6e7f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6e7f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6e7f-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a6e7f-116">Not Supported</span></span>        |
| <span data-ttu-id="a6e7f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6e7f-117">Application</span></span>     | <span data-ttu-id="a6e7f-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="a6e7f-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="a6e7f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6e7f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="a6e7f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6e7f-120">Request headers</span></span>
| <span data-ttu-id="a6e7f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a6e7f-121">Name</span></span>          | <span data-ttu-id="a6e7f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a6e7f-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a6e7f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6e7f-123">Authorization</span></span> | <span data-ttu-id="a6e7f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6e7f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6e7f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6e7f-126">Request body</span></span>
<span data-ttu-id="a6e7f-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a6e7f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6e7f-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="a6e7f-128">Parameter</span></span>      | <span data-ttu-id="a6e7f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a6e7f-129">Type</span></span>    | <span data-ttu-id="a6e7f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a6e7f-130">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="a6e7f-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="a6e7f-131">clientContext</span></span>  | <span data-ttu-id="a6e7f-132">String</span><span class="sxs-lookup"><span data-stu-id="a6e7f-132">String</span></span>  | <span data-ttu-id="a6e7f-133">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="a6e7f-133">Unique client context string.</span></span> <span data-ttu-id="a6e7f-134">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="a6e7f-134">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="a6e7f-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6e7f-135">Response</span></span>
<span data-ttu-id="a6e7f-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="a6e7f-136">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a6e7f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a6e7f-137">Example</span></span>
<span data-ttu-id="a6e7f-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a6e7f-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a6e7f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6e7f-139">Request</span></span>
<span data-ttu-id="a6e7f-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6e7f-140">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a6e7f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6e7f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6e7f-142">C#</span><span class="sxs-lookup"><span data-stu-id="a6e7f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6e7f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6e7f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6e7f-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a6e7f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a6e7f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6e7f-145">Response</span></span>

> <span data-ttu-id="a6e7f-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6e7f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK

{
  "id": "ea91863c-d0a6-4de0-b73a-4c8d63da5d87",
  "status": "completed",
  "createdDateTime": "2019-07-18T19:52:30Z",
  "lastActionDateTime": "2019-07-18T19:52:31Z",
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54",
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="a6e7f-148">Уведомление о тоновом уведомлении</span><span class="sxs-lookup"><span data-stu-id="a6e7f-148">Notification - Tone notification</span></span>

<span data-ttu-id="a6e7f-149">В уведомлении содержится информация о нажатии тона в ресурсе [тонеинфо](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="a6e7f-149">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
      "changeType": "updated",
      "resource": "/app/calls/421f1100-411f-4a29-8514-dbbb9caff45",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "toneInfo": {
          "@odata.type": "#microsoft.graph.toneInfo",
          "sequenceId": 1,
          "tone": "tone1"
        }
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
  ]
}
-->
