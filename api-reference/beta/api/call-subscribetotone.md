---
title: 'Call: Субскрибетотоне'
description: Подпишитесь на DTMF (многочастотный многочастотный сигнал). Это позволяет получать уведомления, когда пользователь нажимает клавиши в "Диалпад".
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 50ff5f41c7637ebe79771db81889e89f982a0d92
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005943"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="e63b2-104">Call: Субскрибетотоне</span><span class="sxs-lookup"><span data-stu-id="e63b2-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e63b2-105">Подпишитесь на DTMF (многочастотный многочастотный сигнал).</span><span class="sxs-lookup"><span data-stu-id="e63b2-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="e63b2-106">Это позволяет получать уведомления, когда пользователь нажимает клавиши в "Диалпад".</span><span class="sxs-lookup"><span data-stu-id="e63b2-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="e63b2-107">Действие **субскрибетотоне** поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="e63b2-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e63b2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e63b2-108">Permissions</span></span>
<span data-ttu-id="e63b2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e63b2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e63b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e63b2-111">Permission type</span></span> | <span data-ttu-id="e63b2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e63b2-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="e63b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e63b2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e63b2-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e63b2-114">Not Supported</span></span>        |
| <span data-ttu-id="e63b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e63b2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e63b2-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e63b2-116">Not Supported</span></span>        |
| <span data-ttu-id="e63b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e63b2-117">Application</span></span>     | <span data-ttu-id="e63b2-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="e63b2-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="e63b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e63b2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /communications/calls/{id}/subscribeToTone
```
> <span data-ttu-id="e63b2-120">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="e63b2-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e63b2-121">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="e63b2-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e63b2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e63b2-122">Request headers</span></span>
| <span data-ttu-id="e63b2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e63b2-123">Name</span></span>          | <span data-ttu-id="e63b2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e63b2-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e63b2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e63b2-125">Authorization</span></span> | <span data-ttu-id="e63b2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e63b2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e63b2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e63b2-128">Request body</span></span>
<span data-ttu-id="e63b2-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e63b2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e63b2-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="e63b2-130">Parameter</span></span>      | <span data-ttu-id="e63b2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e63b2-131">Type</span></span>    | <span data-ttu-id="e63b2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e63b2-132">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="e63b2-133">Контекст</span><span class="sxs-lookup"><span data-stu-id="e63b2-133">clientContext</span></span>  | <span data-ttu-id="e63b2-134">String</span><span class="sxs-lookup"><span data-stu-id="e63b2-134">String</span></span>  | <span data-ttu-id="e63b2-135">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="e63b2-135">Unique client context string.</span></span> <span data-ttu-id="e63b2-136">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="e63b2-136">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="e63b2-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e63b2-137">Response</span></span>
<span data-ttu-id="e63b2-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e63b2-138">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e63b2-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e63b2-139">Example</span></span>
<span data-ttu-id="e63b2-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e63b2-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e63b2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e63b2-141">Request</span></span>
<span data-ttu-id="e63b2-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e63b2-142">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e63b2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e63b2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e63b2-144">C#</span><span class="sxs-lookup"><span data-stu-id="e63b2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e63b2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e63b2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e63b2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e63b2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e63b2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e63b2-147">Response</span></span>

> <span data-ttu-id="e63b2-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e63b2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/421f1100-411f-4a29-8514-dbbb9caff45a/operations/ea91863c-d0a6-4de0-b73a-4c8d63da5d87
Content-Type: application/json
Content-Length: 259

{
  "id": "ea91863c-d0a6-4de0-b73a-4c8d63da5d87",
  "status": "completed",
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54",
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="e63b2-150">Уведомление о тоновом уведомлении</span><span class="sxs-lookup"><span data-stu-id="e63b2-150">Notification - tone notification</span></span>

<span data-ttu-id="e63b2-151">В уведомлении содержится информация о нажатии тона в ресурсе [тонеинфо](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="e63b2-151">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/421f1100-411f-4a29-8514-dbbb9caff45",
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
