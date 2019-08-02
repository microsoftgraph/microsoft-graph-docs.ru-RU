---
title: 'Call: Плайпромпт'
description: Проигрывать запрос в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fc5c80e633055eb6cc1d1914a756bfb80f4332f9
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062010"
---
# <a name="call-playprompt"></a><span data-ttu-id="68f8e-103">Call: Плайпромпт</span><span class="sxs-lookup"><span data-stu-id="68f8e-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68f8e-104">Проигрывать запрос в вызове.</span><span class="sxs-lookup"><span data-stu-id="68f8e-104">Play a prompt in the call.</span></span>

<span data-ttu-id="68f8e-105">Дополнительные сведения об обработке операций можно найти в статье [коммсоператион](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="68f8e-105">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="68f8e-106">Действие **плайпромпт** поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="68f8e-106">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68f8e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68f8e-107">Permissions</span></span>
<span data-ttu-id="68f8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68f8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68f8e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68f8e-110">Permission type</span></span>                        | <span data-ttu-id="68f8e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68f8e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68f8e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68f8e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="68f8e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68f8e-113">Not Supported.</span></span>                               |
| <span data-ttu-id="68f8e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68f8e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68f8e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68f8e-115">Not Supported.</span></span>                               |
| <span data-ttu-id="68f8e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="68f8e-116">Application</span></span>                            | <span data-ttu-id="68f8e-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="68f8e-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="68f8e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68f8e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="68f8e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68f8e-119">Request headers</span></span>
| <span data-ttu-id="68f8e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="68f8e-120">Name</span></span>          | <span data-ttu-id="68f8e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="68f8e-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="68f8e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68f8e-122">Authorization</span></span> | <span data-ttu-id="68f8e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68f8e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68f8e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68f8e-125">Request body</span></span>
<span data-ttu-id="68f8e-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="68f8e-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="68f8e-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="68f8e-127">Parameter</span></span>      | <span data-ttu-id="68f8e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="68f8e-128">Type</span></span>    |<span data-ttu-id="68f8e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="68f8e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68f8e-130">выдан</span><span class="sxs-lookup"><span data-stu-id="68f8e-130">prompts</span></span>|<span data-ttu-id="68f8e-131">Коллекция Медиапромпт</span><span class="sxs-lookup"><span data-stu-id="68f8e-131">MediaPrompt collection</span></span>| <span data-ttu-id="68f8e-132">В настоящее время поддерживается только один запрос и тип [медиапромпт](../resources/mediaprompt.md) .</span><span class="sxs-lookup"><span data-stu-id="68f8e-132">Currently only a single prompt and of type [MediaPrompt](../resources/mediaprompt.md) is supported.</span></span>|
|<span data-ttu-id="68f8e-133">CNAME</span><span class="sxs-lookup"><span data-stu-id="68f8e-133">loop</span></span>|<span data-ttu-id="68f8e-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="68f8e-134">Boolean</span></span>| <span data-ttu-id="68f8e-135">Значение цикла.</span><span class="sxs-lookup"><span data-stu-id="68f8e-135">The loop value.</span></span> <span data-ttu-id="68f8e-136">Значение true указывает, что цикл должен быть бесконечным.</span><span class="sxs-lookup"><span data-stu-id="68f8e-136">True indicates to loop infinitely.</span></span> <span data-ttu-id="68f8e-137">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="68f8e-137">The default value is false.</span></span> |
|<span data-ttu-id="68f8e-138">Контекст</span><span class="sxs-lookup"><span data-stu-id="68f8e-138">clientContext</span></span>|<span data-ttu-id="68f8e-139">String</span><span class="sxs-lookup"><span data-stu-id="68f8e-139">String</span></span>|<span data-ttu-id="68f8e-140">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="68f8e-140">Unique client context string.</span></span> <span data-ttu-id="68f8e-141">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="68f8e-141">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="68f8e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="68f8e-142">Response</span></span>
<span data-ttu-id="68f8e-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [плайпромптоператион](../resources/playpromptoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68f8e-143">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68f8e-144">Пример</span><span class="sxs-lookup"><span data-stu-id="68f8e-144">Example</span></span>
<span data-ttu-id="68f8e-145">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="68f8e-145">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="68f8e-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="68f8e-146">Request</span></span>
<span data-ttu-id="68f8e-147">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68f8e-147">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68f8e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="68f8e-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
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
      },
    },
  ],
  "loop": false
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68f8e-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="68f8e-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="68f8e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="68f8e-150">Response</span></span>
<span data-ttu-id="68f8e-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68f8e-151">The following is an example of the response.</span></span>

> <span data-ttu-id="68f8e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68f8e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="68f8e-154">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="68f8e-154">Notification - operation completed</span></span>

 ><span data-ttu-id="68f8e-155">**Примечание:** При возникновении бесконечного цикла это уведомление не отправляется.</span><span class="sxs-lookup"><span data-stu-id="68f8e-155">**Note:** If infinite looping occurs, this notification is not sent.</span></span>
 
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
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.playPromptOperation",
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
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
