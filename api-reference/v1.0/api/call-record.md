---
title: 'вызов: recordResponse'
description: Запись короткого голосового ответа звонящего. Это полезно, если бот хочет захватить голосовой ответ от вызываемого после запроса.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8766f2764852354fc178c97bd632db550b183f81
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050586"
---
# <a name="call-recordresponse"></a><span data-ttu-id="1cf48-104">вызов: recordResponse</span><span class="sxs-lookup"><span data-stu-id="1cf48-104">call: recordResponse</span></span>

<span data-ttu-id="1cf48-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cf48-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1cf48-106">Запись короткого голосового ответа звонящего.</span><span class="sxs-lookup"><span data-stu-id="1cf48-106">Records a short audio response from the caller.</span></span>
<span data-ttu-id="1cf48-107">Бот может использовать это для захвата голосового ответа от вызываемого после запроса ответа.</span><span class="sxs-lookup"><span data-stu-id="1cf48-107">A bot can utilize this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="1cf48-108">Дополнительные сведения о том, как обрабатывать операции, просмотрите [commsOperation](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="1cf48-108">For further information on how to handle operations, please review [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="1cf48-109">**Примечание:** Это поддерживается только для [вызовов,](../resources/call.md) которые инициированы с [помощью serviceHostedMediaConfig.](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="1cf48-109">**Note:** This is only supported for [calls](../resources/call.md) which are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="1cf48-110">Это действие не предназначено для записи всего вызова.</span><span class="sxs-lookup"><span data-stu-id="1cf48-110">This action is not intended to record the entire call.</span></span> <span data-ttu-id="1cf48-111">Максимальная продолжительность записи — 2 минуты.</span><span class="sxs-lookup"><span data-stu-id="1cf48-111">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="1cf48-112">Запись не будет постоянно сохранена платформой облачных коммуникаций и удаляется вскоре после окончания вызова.</span><span class="sxs-lookup"><span data-stu-id="1cf48-112">The recording is not saved permanently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="1cf48-113">Бот должен быстро скачать запись после завершения операции записи, используя значение recordingLocation, которое дано в завершенной уведомлении.</span><span class="sxs-lookup"><span data-stu-id="1cf48-113">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="1cf48-114">**Примечание:** Любые собранные средства **массовой** информации не могут сохраняться.</span><span class="sxs-lookup"><span data-stu-id="1cf48-114">**Note:** Any media collected may **not** be persisted.</span></span> <span data-ttu-id="1cf48-115">Убедитесь, что вы соответствуете законам и правилам вашей области, когда дело доходит до записи вызовов.</span><span class="sxs-lookup"><span data-stu-id="1cf48-115">Make sure you are compliant with the laws and regulations of your area when it comes to call recording.</span></span> <span data-ttu-id="1cf48-116">Дополнительные сведения обратитесь к адвокату.</span><span class="sxs-lookup"><span data-stu-id="1cf48-116">Please consult with a legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cf48-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1cf48-117">Permissions</span></span>
<span data-ttu-id="1cf48-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cf48-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cf48-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cf48-120">Permission type</span></span> | <span data-ttu-id="1cf48-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cf48-121">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="1cf48-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cf48-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cf48-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1cf48-123">Not Supported</span></span>        |
| <span data-ttu-id="1cf48-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cf48-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cf48-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1cf48-125">Not Supported</span></span>        |
| <span data-ttu-id="1cf48-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cf48-126">Application</span></span>     | <span data-ttu-id="1cf48-127">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="1cf48-127">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="1cf48-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cf48-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/recordResponse
```

## <a name="request-headers"></a><span data-ttu-id="1cf48-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cf48-129">Request headers</span></span>
| <span data-ttu-id="1cf48-130">Имя</span><span class="sxs-lookup"><span data-stu-id="1cf48-130">Name</span></span>          | <span data-ttu-id="1cf48-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf48-131">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1cf48-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cf48-132">Authorization</span></span> | <span data-ttu-id="1cf48-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cf48-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cf48-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cf48-135">Request body</span></span>
<span data-ttu-id="1cf48-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1cf48-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1cf48-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="1cf48-137">Parameter</span></span>      | <span data-ttu-id="1cf48-138">Тип</span><span class="sxs-lookup"><span data-stu-id="1cf48-138">Type</span></span>    |<span data-ttu-id="1cf48-139">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf48-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cf48-140">подсказки</span><span class="sxs-lookup"><span data-stu-id="1cf48-140">prompts</span></span>|<span data-ttu-id="1cf48-141">[коллекция mediaPrompt](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="1cf48-141">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="1cf48-142">Подсказки для игры.</span><span class="sxs-lookup"><span data-stu-id="1cf48-142">The prompts to be played.</span></span> <span data-ttu-id="1cf48-143">Максимальный поддерживаемый размер коллекции mediaPrompt — 1.</span><span class="sxs-lookup"><span data-stu-id="1cf48-143">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="1cf48-144">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="1cf48-144">bargeInAllowed</span></span>|<span data-ttu-id="1cf48-145">Логический</span><span class="sxs-lookup"><span data-stu-id="1cf48-145">Boolean</span></span>| <span data-ttu-id="1cf48-146">Если это так, запрос recordResponse будет вступать в другие существующие запросы записи и записи playprompt в очереди или в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="1cf48-146">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="1cf48-147">По умолчанию = false.</span><span class="sxs-lookup"><span data-stu-id="1cf48-147">Default = false.</span></span> |
|<span data-ttu-id="1cf48-148">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="1cf48-148">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="1cf48-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1cf48-149">Int32</span></span>| <span data-ttu-id="1cf48-150">Максимальная начальная тишина (тишина пользователя) разрешена с того времени, когда мы начнем операцию записи ответа перед периодиалом и не справимся с операцией.</span><span class="sxs-lookup"><span data-stu-id="1cf48-150">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="1cf48-151">Если мы играем запрос, этот отсвечив начинается после завершения запроса.</span><span class="sxs-lookup"><span data-stu-id="1cf48-151">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="1cf48-152">По умолчанию = 5 секунд, Min = 1 секунда, Max = 120 секунд</span><span class="sxs-lookup"><span data-stu-id="1cf48-152">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="1cf48-153">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="1cf48-153">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="1cf48-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1cf48-154">Int32</span></span>| <span data-ttu-id="1cf48-155">Максимальное время тишины (паузы) после начала выступления пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cf48-155">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="1cf48-156">По умолчанию = 5 секунд, Min = 1 секунда, Max = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="1cf48-156">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="1cf48-157">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="1cf48-157">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="1cf48-158">Int32</span><span class="sxs-lookup"><span data-stu-id="1cf48-158">Int32</span></span>| <span data-ttu-id="1cf48-159">Максимальная продолжительность операции recordResponse перед остановкой записи.</span><span class="sxs-lookup"><span data-stu-id="1cf48-159">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="1cf48-160">По умолчанию = 5 секунд, Min = 1 секунда, Max = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="1cf48-160">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="1cf48-161">playBeep</span><span class="sxs-lookup"><span data-stu-id="1cf48-161">playBeep</span></span>|<span data-ttu-id="1cf48-162">Логический</span><span class="sxs-lookup"><span data-stu-id="1cf48-162">Boolean</span></span>| <span data-ttu-id="1cf48-163">Если это так, воспроизводит звуковой сигнал, чтобы указать пользователю, что он может начать запись своего сообщения.</span><span class="sxs-lookup"><span data-stu-id="1cf48-163">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="1cf48-164">По умолчанию = true.</span><span class="sxs-lookup"><span data-stu-id="1cf48-164">Default = true.</span></span>|
|<span data-ttu-id="1cf48-165">stopTones</span><span class="sxs-lookup"><span data-stu-id="1cf48-165">stopTones</span></span>|<span data-ttu-id="1cf48-166">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1cf48-166">String collection</span></span>|<span data-ttu-id="1cf48-167">Стоп-сигналы, указанные для окончания записи.</span><span class="sxs-lookup"><span data-stu-id="1cf48-167">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="1cf48-168">clientContext</span><span class="sxs-lookup"><span data-stu-id="1cf48-168">clientContext</span></span>|<span data-ttu-id="1cf48-169">String</span><span class="sxs-lookup"><span data-stu-id="1cf48-169">String</span></span>|<span data-ttu-id="1cf48-170">Уникальная строка Client Context.</span><span class="sxs-lookup"><span data-stu-id="1cf48-170">Unique Client Context string.</span></span> <span data-ttu-id="1cf48-171">Максимальное ограничение — 256 шаров.</span><span class="sxs-lookup"><span data-stu-id="1cf48-171">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="1cf48-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cf48-172">Response</span></span>
<span data-ttu-id="1cf48-173">Этот метод возвращает код ответа и заглавную ссылку Location с URI в `200 OK` [записьОперацией,](../resources/recordoperation.md) созданной для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="1cf48-173">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="1cf48-174">Пример</span><span class="sxs-lookup"><span data-stu-id="1cf48-174">Example</span></span>
<span data-ttu-id="1cf48-175">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="1cf48-175">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="1cf48-176">Пример 1. Запись короткого звукового ответа от вызываемой стороны</span><span class="sxs-lookup"><span data-stu-id="1cf48-176">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="1cf48-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cf48-177">Request</span></span>
<span data-ttu-id="1cf48-178">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cf48-178">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1cf48-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cf48-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-recordResponse"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/recordResponse
Content-Type: application/json
Content-Length: 394

{
  "bargeInAllowed": true,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      }
    }
  ],
  "maxRecordDurationInSeconds": 10,
  "initialSilenceTimeoutInSeconds": 5,
  "maxSilenceTimeoutInSeconds": 2,
  "playBeep": true,
  "stopTones": [ "#", "1", "*" ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="1cf48-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cf48-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1cf48-181">C#</span><span class="sxs-lookup"><span data-stu-id="1cf48-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cf48-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cf48-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cf48-183">Java</span><span class="sxs-lookup"><span data-stu-id="1cf48-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-recordresponse-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1cf48-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cf48-184">Response</span></span>
<span data-ttu-id="1cf48-185">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1cf48-185">The following example shows the response.</span></span>

> <span data-ttu-id="1cf48-186">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1cf48-186">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="1cf48-187">Уведомление — операция завершена</span><span class="sxs-lookup"><span data-stu-id="1cf48-187">Notification - operation completed</span></span>

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
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 200,
          "subcode": 8515,
          "message": "Action completed, max record duration reached."
        },
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>"
      }
    }
  ]
}
```

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="1cf48-188">Пример 2. Ирисовка файла записи</span><span class="sxs-lookup"><span data-stu-id="1cf48-188">Example 2: Retrieving the recording file</span></span>

><span data-ttu-id="1cf48-189">**Примечание:** Вы не можете записывать или иным образом сохранять медиаконтент из звонков или собраний, к которые ваше приложение имеет доступ, или данных, полученных из этого медиаконтента.</span><span class="sxs-lookup"><span data-stu-id="1cf48-189">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="1cf48-190">Убедитесь, что вы соответствуете законам и правилам вашей области в отношении защиты данных и конфиденциальности сообщений.</span><span class="sxs-lookup"><span data-stu-id="1cf48-190">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="1cf48-191">Дополнительные сведения можно узнать из [условий использования](/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="1cf48-191">Please see the [Terms of Use](/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="1cf48-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cf48-192">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="1cf48-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cf48-193">Response</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Transfer-Encoding: chunked
Date: Thu, 17 Jan 2019 01:46:37 GMT
Content-Type: application/octet-stream

(application/octet-stream of size 160696 bytes)
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
