---
title: 'вызов: subscribeToTone'
description: Подписка на DTMF (двухтонная многочастотная сигнализация). Это позволяет вам быть уведомленным, когда пользователь нажимает клавиши на "Dialpad".
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7fb6cbbea2ff3e90f7e0b9ed33b79666146e8ec5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047625"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="648a2-104">вызов: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="648a2-104">call: subscribeToTone</span></span>

<span data-ttu-id="648a2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="648a2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="648a2-106">Подписка на DTMF (двухтонная многочастотная сигнализация).</span><span class="sxs-lookup"><span data-stu-id="648a2-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="648a2-107">Это позволяет вам быть уведомленным, когда пользователь нажимает клавиши на "Dialpad".</span><span class="sxs-lookup"><span data-stu-id="648a2-107">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="648a2-108">Действие **subscribeToTone** поддерживается только [для](../resources/call.md) звонков, инициированных с помощью [serviceHostedMediaConfig.](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="648a2-108">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="648a2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="648a2-109">Permissions</span></span>
<span data-ttu-id="648a2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="648a2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="648a2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="648a2-112">Permission type</span></span> | <span data-ttu-id="648a2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="648a2-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="648a2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="648a2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="648a2-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="648a2-115">Not Supported</span></span>        |
| <span data-ttu-id="648a2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="648a2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="648a2-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="648a2-117">Not Supported</span></span>        |
| <span data-ttu-id="648a2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="648a2-118">Application</span></span>     | <span data-ttu-id="648a2-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="648a2-119">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="648a2-120">**Примечание:** Любые предоставленные данные тона могут не сохраняться.</span><span class="sxs-lookup"><span data-stu-id="648a2-120">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="648a2-121">Убедитесь, что вы соответствуете законам и правилам вашей области в отношении защиты данных и конфиденциальности сообщений.</span><span class="sxs-lookup"><span data-stu-id="648a2-121">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="648a2-122">Дополнительные сведения можно узнать из [условий использования](/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="648a2-122">Please see the [Terms of Use](/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>
## <a name="http-request"></a><span data-ttu-id="648a2-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="648a2-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /communications/calls/{id}/subscribeToTone
```
> <span data-ttu-id="648a2-124">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="648a2-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="648a2-125">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="648a2-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="648a2-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="648a2-126">Request headers</span></span>
| <span data-ttu-id="648a2-127">Имя</span><span class="sxs-lookup"><span data-stu-id="648a2-127">Name</span></span>          | <span data-ttu-id="648a2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="648a2-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="648a2-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="648a2-129">Authorization</span></span> | <span data-ttu-id="648a2-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="648a2-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="648a2-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="648a2-132">Request body</span></span>
<span data-ttu-id="648a2-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="648a2-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="648a2-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="648a2-134">Parameter</span></span>      | <span data-ttu-id="648a2-135">Тип</span><span class="sxs-lookup"><span data-stu-id="648a2-135">Type</span></span>    | <span data-ttu-id="648a2-136">Описание</span><span class="sxs-lookup"><span data-stu-id="648a2-136">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="648a2-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="648a2-137">clientContext</span></span>  | <span data-ttu-id="648a2-138">String</span><span class="sxs-lookup"><span data-stu-id="648a2-138">String</span></span>  | <span data-ttu-id="648a2-139">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="648a2-139">Unique client context string.</span></span> <span data-ttu-id="648a2-140">Может иметь не более 256 символов.</span><span class="sxs-lookup"><span data-stu-id="648a2-140">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="648a2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="648a2-141">Response</span></span>
<span data-ttu-id="648a2-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="648a2-142">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="648a2-143">Пример</span><span class="sxs-lookup"><span data-stu-id="648a2-143">Example</span></span>
<span data-ttu-id="648a2-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="648a2-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="648a2-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="648a2-145">Request</span></span>
<span data-ttu-id="648a2-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="648a2-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="648a2-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="648a2-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="648a2-148">C#</span><span class="sxs-lookup"><span data-stu-id="648a2-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="648a2-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="648a2-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="648a2-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="648a2-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="648a2-151">Java</span><span class="sxs-lookup"><span data-stu-id="648a2-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-subscribetotone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="648a2-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="648a2-152">Response</span></span>

> <span data-ttu-id="648a2-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="648a2-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-subscribeToTone",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.subscribeToToneOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="648a2-154">Уведомление — уведомление о тоне</span><span class="sxs-lookup"><span data-stu-id="648a2-154">Notification - tone notification</span></span>

<span data-ttu-id="648a2-155">Уведомление содержит сведения о тоне, нажатом в [ресурсе toneinfo.](../resources/toneinfo.md)</span><span class="sxs-lookup"><span data-stu-id="648a2-155">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
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
