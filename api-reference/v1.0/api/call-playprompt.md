---
title: 'Call: Плайпромпт'
description: Проигрывать запрос в вызове.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 527797215da0ef961c83679fcec313c183a1cd63
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682194"
---
# <a name="call-playprompt"></a><span data-ttu-id="688cd-103">Call: Плайпромпт</span><span class="sxs-lookup"><span data-stu-id="688cd-103">call: playPrompt</span></span>

<span data-ttu-id="688cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="688cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="688cd-105">Проигрывать запрос в вызове.</span><span class="sxs-lookup"><span data-stu-id="688cd-105">Play a prompt in the call.</span></span>

<span data-ttu-id="688cd-106">Дополнительные сведения об обработке операций можно найти в статье [коммсоператион](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="688cd-106">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="688cd-107">Действие **плайпромпт** поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="688cd-107">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="688cd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="688cd-108">Permissions</span></span>
<span data-ttu-id="688cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="688cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="688cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="688cd-111">Permission type</span></span>                        | <span data-ttu-id="688cd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="688cd-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="688cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="688cd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="688cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="688cd-114">Not Supported.</span></span>                               |
| <span data-ttu-id="688cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="688cd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="688cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="688cd-116">Not Supported.</span></span>                               |
| <span data-ttu-id="688cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="688cd-117">Application</span></span>                            | <span data-ttu-id="688cd-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="688cd-118">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="688cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="688cd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="688cd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="688cd-120">Request headers</span></span>
| <span data-ttu-id="688cd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="688cd-121">Name</span></span>          | <span data-ttu-id="688cd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="688cd-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="688cd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="688cd-123">Authorization</span></span> | <span data-ttu-id="688cd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="688cd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="688cd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="688cd-126">Request body</span></span>
<span data-ttu-id="688cd-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="688cd-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="688cd-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="688cd-128">Parameter</span></span>      | <span data-ttu-id="688cd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="688cd-129">Type</span></span>    |<span data-ttu-id="688cd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="688cd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="688cd-131">выдан</span><span class="sxs-lookup"><span data-stu-id="688cd-131">prompts</span></span>|<span data-ttu-id="688cd-132">Коллекция [медиапромпт](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="688cd-132">[MediaPrompt](../resources/mediaprompt.md) collection</span></span>| <span data-ttu-id="688cd-133">Приглашения для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="688cd-133">The prompts to be played.</span></span> <span data-ttu-id="688cd-134">Максимальный поддерживаемый размер коллекции Медиапромпт составляет 20.</span><span class="sxs-lookup"><span data-stu-id="688cd-134">The maximum supported MediaPrompt collection size is 20.</span></span>|
|<span data-ttu-id="688cd-135">Контекст</span><span class="sxs-lookup"><span data-stu-id="688cd-135">clientContext</span></span>|<span data-ttu-id="688cd-136">String</span><span class="sxs-lookup"><span data-stu-id="688cd-136">String</span></span>|<span data-ttu-id="688cd-137">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="688cd-137">Unique client context string.</span></span> <span data-ttu-id="688cd-138">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="688cd-138">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="688cd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="688cd-139">Response</span></span>
<span data-ttu-id="688cd-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [плайпромптоператион](../resources/playpromptoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="688cd-140">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="688cd-141">Пример</span><span class="sxs-lookup"><span data-stu-id="688cd-141">Example</span></span>
<span data-ttu-id="688cd-142">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="688cd-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="688cd-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="688cd-143">Request</span></span>
<span data-ttu-id="688cd-144">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="688cd-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="688cd-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="688cd-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "@odata.type": "#microsoft.graph.mediaInfo",
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      }
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="688cd-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="688cd-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="688cd-147">C#</span><span class="sxs-lookup"><span data-stu-id="688cd-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-playprompt-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="688cd-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="688cd-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-playprompt-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="688cd-149">Java</span><span class="sxs-lookup"><span data-stu-id="688cd-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-playprompt-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="688cd-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="688cd-150">Response</span></span>
<span data-ttu-id="688cd-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="688cd-151">The following is an example of the response.</span></span>

> <span data-ttu-id="688cd-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="688cd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="688cd-154">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="688cd-154">Notification - operation completed</span></span>
 
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
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.playPromptOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 200,
          "subcode": 0,
          "message": "Action completed successfully."
        },
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
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
