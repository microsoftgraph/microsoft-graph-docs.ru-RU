---
title: 'Call: Субскрибетотоне'
description: Подпишитесь на DTMF (многочастотный многочастотный сигнал). Это позволяет получать уведомления, когда пользователь нажимает клавиши в "Диалпад".
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 45b2145c002eb17a5bc65f946646ce70bf3872f8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518667"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="2cdb8-104">Call: Субскрибетотоне</span><span class="sxs-lookup"><span data-stu-id="2cdb8-104">call: subscribeToTone</span></span>

<span data-ttu-id="2cdb8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cdb8-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="2cdb8-106">Подпишитесь на DTMF (многочастотный многочастотный сигнал).</span><span class="sxs-lookup"><span data-stu-id="2cdb8-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="2cdb8-107">Это позволяет получать уведомления, когда пользователь нажимает клавиши в "диалпад".</span><span class="sxs-lookup"><span data-stu-id="2cdb8-107">This allows you to be notified when the user presses keys on a "dialpad".</span></span>

> [!Note]
> <span data-ttu-id="2cdb8-108">Действие **субскрибетотоне** поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="2cdb8-108">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2cdb8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2cdb8-109">Permissions</span></span>
<span data-ttu-id="2cdb8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cdb8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2cdb8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cdb8-112">Permission type</span></span> | <span data-ttu-id="2cdb8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cdb8-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="2cdb8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cdb8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2cdb8-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2cdb8-115">Not Supported</span></span>        |
| <span data-ttu-id="2cdb8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cdb8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cdb8-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2cdb8-117">Not Supported</span></span>        |
| <span data-ttu-id="2cdb8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cdb8-118">Application</span></span>     | <span data-ttu-id="2cdb8-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="2cdb8-119">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="2cdb8-120">**Примечание:** Все указанные данные тона могут быть не сохранены.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-120">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="2cdb8-121">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-121">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="2cdb8-122">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-122">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="http-request"></a><span data-ttu-id="2cdb8-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cdb8-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="2cdb8-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cdb8-124">Request headers</span></span>
| <span data-ttu-id="2cdb8-125">Имя</span><span class="sxs-lookup"><span data-stu-id="2cdb8-125">Name</span></span>          | <span data-ttu-id="2cdb8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="2cdb8-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2cdb8-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cdb8-127">Authorization</span></span> | <span data-ttu-id="2cdb8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cdb8-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2cdb8-130">Request body</span></span>
<span data-ttu-id="2cdb8-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2cdb8-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="2cdb8-132">Parameter</span></span>      | <span data-ttu-id="2cdb8-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2cdb8-133">Type</span></span>    | <span data-ttu-id="2cdb8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2cdb8-134">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="2cdb8-135">Контекст</span><span class="sxs-lookup"><span data-stu-id="2cdb8-135">clientContext</span></span>  | <span data-ttu-id="2cdb8-136">String</span><span class="sxs-lookup"><span data-stu-id="2cdb8-136">String</span></span>  | <span data-ttu-id="2cdb8-137">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-137">Unique client context string.</span></span> <span data-ttu-id="2cdb8-138">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-138">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="2cdb8-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cdb8-139">Response</span></span>
<span data-ttu-id="2cdb8-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-140">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2cdb8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2cdb8-141">Example</span></span>
<span data-ttu-id="2cdb8-142">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2cdb8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cdb8-143">Request</span></span>
<span data-ttu-id="2cdb8-144">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2cdb8-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cdb8-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="c"></a>[<span data-ttu-id="2cdb8-146">C#</span><span class="sxs-lookup"><span data-stu-id="2cdb8-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cdb8-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cdb8-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cdb8-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cdb8-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2cdb8-149">Java</span><span class="sxs-lookup"><span data-stu-id="2cdb8-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-subscribetotone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2cdb8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cdb8-150">Response</span></span>

> <span data-ttu-id="2cdb8-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cdb8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-subscribeToTone",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.subscribeToToneOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "completed"
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="2cdb8-153">Уведомление о тоновом уведомлении</span><span class="sxs-lookup"><span data-stu-id="2cdb8-153">Notification - tone notification</span></span>

<span data-ttu-id="2cdb8-154">В уведомлении содержится информация о нажатии тона в ресурсе [тонеинфо](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="2cdb8-154">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
