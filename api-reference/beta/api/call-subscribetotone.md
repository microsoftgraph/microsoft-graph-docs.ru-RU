---
title: 'Call: Субскрибетотоне'
description: Подпишитесь на DTMF (многочастотный многочастотный сигнал). Это позволяет получать уведомления, когда пользователь нажимает клавиши в "Диалпад".
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4aade47d641cbeb129b199858956f144e2d4bd0d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912750"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="55a70-104">Call: Субскрибетотоне</span><span class="sxs-lookup"><span data-stu-id="55a70-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55a70-105">Подпишитесь на DTMF (многочастотный многочастотный сигнал).</span><span class="sxs-lookup"><span data-stu-id="55a70-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="55a70-106">Это позволяет получать уведомления, когда пользователь нажимает клавиши в "Диалпад".</span><span class="sxs-lookup"><span data-stu-id="55a70-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="55a70-107">Действие **субскрибетотоне** поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="55a70-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="55a70-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55a70-108">Permissions</span></span>
<span data-ttu-id="55a70-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55a70-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55a70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55a70-111">Permission type</span></span> | <span data-ttu-id="55a70-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55a70-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="55a70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55a70-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="55a70-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="55a70-114">Not Supported</span></span>        |
| <span data-ttu-id="55a70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55a70-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55a70-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="55a70-116">Not Supported</span></span>        |
| <span data-ttu-id="55a70-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55a70-117">Application</span></span>     | <span data-ttu-id="55a70-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="55a70-118">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="55a70-119">**Примечание:** Все указанные данные тона могут быть не сохранены.</span><span class="sxs-lookup"><span data-stu-id="55a70-119">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="55a70-120">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="55a70-120">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="55a70-121">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="55a70-121">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>
## <a name="http-request"></a><span data-ttu-id="55a70-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55a70-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /communications/calls/{id}/subscribeToTone
```
> <span data-ttu-id="55a70-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="55a70-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="55a70-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="55a70-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55a70-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55a70-125">Request headers</span></span>
| <span data-ttu-id="55a70-126">Имя</span><span class="sxs-lookup"><span data-stu-id="55a70-126">Name</span></span>          | <span data-ttu-id="55a70-127">Описание</span><span class="sxs-lookup"><span data-stu-id="55a70-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="55a70-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55a70-128">Authorization</span></span> | <span data-ttu-id="55a70-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55a70-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55a70-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55a70-131">Request body</span></span>
<span data-ttu-id="55a70-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="55a70-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55a70-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="55a70-133">Parameter</span></span>      | <span data-ttu-id="55a70-134">Тип</span><span class="sxs-lookup"><span data-stu-id="55a70-134">Type</span></span>    | <span data-ttu-id="55a70-135">Описание</span><span class="sxs-lookup"><span data-stu-id="55a70-135">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="55a70-136">Контекст</span><span class="sxs-lookup"><span data-stu-id="55a70-136">clientContext</span></span>  | <span data-ttu-id="55a70-137">String</span><span class="sxs-lookup"><span data-stu-id="55a70-137">String</span></span>  | <span data-ttu-id="55a70-138">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="55a70-138">Unique client context string.</span></span> <span data-ttu-id="55a70-139">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="55a70-139">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="55a70-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="55a70-140">Response</span></span>
<span data-ttu-id="55a70-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="55a70-141">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="55a70-142">Пример</span><span class="sxs-lookup"><span data-stu-id="55a70-142">Example</span></span>
<span data-ttu-id="55a70-143">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="55a70-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="55a70-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="55a70-144">Request</span></span>
<span data-ttu-id="55a70-145">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55a70-145">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="55a70-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="55a70-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="55a70-147">C#</span><span class="sxs-lookup"><span data-stu-id="55a70-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55a70-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55a70-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55a70-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55a70-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55a70-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="55a70-150">Response</span></span>

> <span data-ttu-id="55a70-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55a70-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


##### <a name="notification---tone-notification"></a><span data-ttu-id="55a70-153">Уведомление о тоновом уведомлении</span><span class="sxs-lookup"><span data-stu-id="55a70-153">Notification - tone notification</span></span>

<span data-ttu-id="55a70-154">В уведомлении содержится информация о нажатии тона в ресурсе [тонеинфо](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="55a70-154">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
