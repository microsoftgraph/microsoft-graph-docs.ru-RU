---
title: 'Call: Субскрибетотоне'
description: Подпишитесь на DTMF (многочастотный многочастотный сигнал). Это позволяет получать уведомления, когда пользователь нажимает клавиши в "Диалпад".
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: aea175602f363477103fba7b6fad785ce4f22c5f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987297"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="b5410-104">Call: Субскрибетотоне</span><span class="sxs-lookup"><span data-stu-id="b5410-104">call: subscribeToTone</span></span>

<span data-ttu-id="b5410-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5410-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5410-106">Подпишитесь на DTMF (многочастотный многочастотный сигнал).</span><span class="sxs-lookup"><span data-stu-id="b5410-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="b5410-107">Это позволяет получать уведомления, когда пользователь нажимает клавиши в "Диалпад".</span><span class="sxs-lookup"><span data-stu-id="b5410-107">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="b5410-108">Действие **субскрибетотоне** поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="b5410-108">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5410-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5410-109">Permissions</span></span>
<span data-ttu-id="b5410-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5410-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5410-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5410-112">Permission type</span></span> | <span data-ttu-id="b5410-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5410-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="b5410-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5410-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5410-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5410-115">Not Supported</span></span>        |
| <span data-ttu-id="b5410-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5410-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5410-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5410-117">Not Supported</span></span>        |
| <span data-ttu-id="b5410-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5410-118">Application</span></span>     | <span data-ttu-id="b5410-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="b5410-119">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="b5410-120">**Примечание:** Все указанные данные тона могут быть не сохранены.</span><span class="sxs-lookup"><span data-stu-id="b5410-120">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="b5410-121">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="b5410-121">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="b5410-122">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="b5410-122">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>
## <a name="http-request"></a><span data-ttu-id="b5410-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5410-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /communications/calls/{id}/subscribeToTone
```
> <span data-ttu-id="b5410-124">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="b5410-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="b5410-125">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="b5410-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5410-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5410-126">Request headers</span></span>
| <span data-ttu-id="b5410-127">Имя</span><span class="sxs-lookup"><span data-stu-id="b5410-127">Name</span></span>          | <span data-ttu-id="b5410-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b5410-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b5410-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5410-129">Authorization</span></span> | <span data-ttu-id="b5410-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5410-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5410-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b5410-132">Request body</span></span>
<span data-ttu-id="b5410-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b5410-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b5410-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="b5410-134">Parameter</span></span>      | <span data-ttu-id="b5410-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b5410-135">Type</span></span>    | <span data-ttu-id="b5410-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b5410-136">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="b5410-137">Контекст</span><span class="sxs-lookup"><span data-stu-id="b5410-137">clientContext</span></span>  | <span data-ttu-id="b5410-138">String</span><span class="sxs-lookup"><span data-stu-id="b5410-138">String</span></span>  | <span data-ttu-id="b5410-139">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="b5410-139">Unique client context string.</span></span> <span data-ttu-id="b5410-140">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="b5410-140">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="b5410-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5410-141">Response</span></span>
<span data-ttu-id="b5410-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b5410-142">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b5410-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b5410-143">Example</span></span>
<span data-ttu-id="b5410-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b5410-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b5410-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5410-145">Request</span></span>
<span data-ttu-id="b5410-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5410-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b5410-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5410-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b5410-148">C#</span><span class="sxs-lookup"><span data-stu-id="b5410-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5410-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5410-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5410-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5410-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5410-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5410-151">Response</span></span>

> <span data-ttu-id="b5410-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5410-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


##### <a name="notification---tone-notification"></a><span data-ttu-id="b5410-154">Уведомление о тоновом уведомлении</span><span class="sxs-lookup"><span data-stu-id="b5410-154">Notification - tone notification</span></span>

<span data-ttu-id="b5410-155">В уведомлении содержится информация о нажатии тона в ресурсе [тонеинфо](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="b5410-155">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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


