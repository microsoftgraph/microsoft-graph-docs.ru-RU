---
title: 'Call: Рекордреспонсе'
description: Запишите короткий звуковой ответ от вызывающего абонента. Это полезно, если Bot хочет записать голосовой ответ от абонента, вызываемого после приглашения.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6c8038c0f2bea125de882c5007954890bbecac5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987307"
---
# <a name="call-recordresponse"></a><span data-ttu-id="f204d-104">Call: Рекордреспонсе</span><span class="sxs-lookup"><span data-stu-id="f204d-104">call: recordResponse</span></span>

<span data-ttu-id="f204d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f204d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f204d-106">Запишите короткий звуковой ответ от вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="f204d-106">Record a short audio response from the caller.</span></span>

<span data-ttu-id="f204d-107">С помощью Bot можно получить голосовой ответ от вызывающего абонента после получения запроса на ответ.</span><span class="sxs-lookup"><span data-stu-id="f204d-107">A bot can use this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="f204d-108">Дополнительные сведения об обработке операций можно найти в статье [коммсоператион](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="f204d-108">For more information about how to handle operations, see [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="f204d-109">**Примечание:** Этот API поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="f204d-109">**Note:** This API is only supported for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="f204d-110">Это действие не предназначено для записи всего вызова.</span><span class="sxs-lookup"><span data-stu-id="f204d-110">This action is not intended to record the entire call.</span></span> <span data-ttu-id="f204d-111">Максимальная длина записи составляет 2 минуты.</span><span class="sxs-lookup"><span data-stu-id="f204d-111">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="f204d-112">Запись не сохраняется окончательно при помощи платформы Cloud Communications и удаляется вскоре после завершения вызова.</span><span class="sxs-lookup"><span data-stu-id="f204d-112">The recording is not saved permanently by the by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="f204d-113">Bot должен сразу скачать запись после завершения операции записи, используя значение Рекординглокатион, указанное в завершенном уведомлении.</span><span class="sxs-lookup"><span data-stu-id="f204d-113">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="f204d-114">**Примечание:** Вы не можете записать или оставить мультимедийный контент из звонков или собраний, к которым обращается приложение, или данных, полученных из этого контента.</span><span class="sxs-lookup"><span data-stu-id="f204d-114">**Note:** You may not record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="f204d-115">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="f204d-115">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="f204d-116">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="f204d-116">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="f204d-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f204d-117">Permissions</span></span>
<span data-ttu-id="f204d-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f204d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f204d-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f204d-120">Permission type</span></span> | <span data-ttu-id="f204d-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f204d-121">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="f204d-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f204d-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="f204d-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f204d-123">Not Supported</span></span>        |
| <span data-ttu-id="f204d-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f204d-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f204d-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f204d-125">Not Supported</span></span>        |
| <span data-ttu-id="f204d-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f204d-126">Application</span></span>     | <span data-ttu-id="f204d-127">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="f204d-127">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="f204d-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f204d-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/recordResponse
POST /communications/calls/{id}/recordResponse
```
> <span data-ttu-id="f204d-129">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="f204d-129">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="f204d-130">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="f204d-130">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f204d-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f204d-131">Request headers</span></span>
| <span data-ttu-id="f204d-132">Имя</span><span class="sxs-lookup"><span data-stu-id="f204d-132">Name</span></span>          | <span data-ttu-id="f204d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f204d-133">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f204d-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f204d-134">Authorization</span></span> | <span data-ttu-id="f204d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f204d-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f204d-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f204d-137">Content-type</span></span>| <span data-ttu-id="f204d-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f204d-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f204d-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f204d-140">Request body</span></span>
<span data-ttu-id="f204d-141">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f204d-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f204d-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="f204d-142">Parameter</span></span>      | <span data-ttu-id="f204d-143">Тип</span><span class="sxs-lookup"><span data-stu-id="f204d-143">Type</span></span>    |<span data-ttu-id="f204d-144">Описание</span><span class="sxs-lookup"><span data-stu-id="f204d-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f204d-145">выдан</span><span class="sxs-lookup"><span data-stu-id="f204d-145">prompts</span></span>|<span data-ttu-id="f204d-146">Коллекция [медиапромпт](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="f204d-146">[MediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="f204d-147">Приглашения для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="f204d-147">The prompts to be played.</span></span> <span data-ttu-id="f204d-148">Максимальный поддерживаемый размер коллекции Медиапромпт составляет 1.</span><span class="sxs-lookup"><span data-stu-id="f204d-148">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="f204d-149">баржеиналловед</span><span class="sxs-lookup"><span data-stu-id="f204d-149">bargeInAllowed</span></span>|<span data-ttu-id="f204d-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="f204d-150">Boolean</span></span>| <span data-ttu-id="f204d-151">Если этот параметр имеет значение true, запрос Рекордреспонсе будет барже в другие существующие запросы записи или плайпромпт в очереди.</span><span class="sxs-lookup"><span data-stu-id="f204d-151">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="f204d-152">Значение по умолчанию = false.</span><span class="sxs-lookup"><span data-stu-id="f204d-152">Default = false.</span></span> |
|<span data-ttu-id="f204d-153">инитиалсиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="f204d-153">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="f204d-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f204d-154">Int32</span></span>| <span data-ttu-id="f204d-155">Максимальное значение параметра "тишина" (тишина пользователя) разрешено с момента запуска операции записи ответа до истечения времени ожидания и сбоев операции.</span><span class="sxs-lookup"><span data-stu-id="f204d-155">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="f204d-156">При воспроизведении приглашения этот таймер запускается после завершения приглашения.</span><span class="sxs-lookup"><span data-stu-id="f204d-156">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="f204d-157">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд</span><span class="sxs-lookup"><span data-stu-id="f204d-157">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="f204d-158">макссиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="f204d-158">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="f204d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="f204d-159">Int32</span></span>| <span data-ttu-id="f204d-160">Максимально допустимое время тишины (пауза) после начала диктовки пользователя.</span><span class="sxs-lookup"><span data-stu-id="f204d-160">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="f204d-161">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="f204d-161">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="f204d-162">максрекорддуратионинсекондс</span><span class="sxs-lookup"><span data-stu-id="f204d-162">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="f204d-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f204d-163">Int32</span></span>| <span data-ttu-id="f204d-164">Максимальная длительность операции Рекордреспонсе перед остановкой записи.</span><span class="sxs-lookup"><span data-stu-id="f204d-164">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="f204d-165">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="f204d-165">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="f204d-166">плайбип</span><span class="sxs-lookup"><span data-stu-id="f204d-166">playBeep</span></span>|<span data-ttu-id="f204d-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f204d-167">Boolean</span></span>| <span data-ttu-id="f204d-168">Если этот параметр имеет значение true, воспроизводит звуковой сигнал, указывающий пользователю, что он может начать запись сообщения.</span><span class="sxs-lookup"><span data-stu-id="f204d-168">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="f204d-169">Значение по умолчанию = true.</span><span class="sxs-lookup"><span data-stu-id="f204d-169">Default = true.</span></span>|
|<span data-ttu-id="f204d-170">стоптонес</span><span class="sxs-lookup"><span data-stu-id="f204d-170">stopTones</span></span>|<span data-ttu-id="f204d-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f204d-171">String collection</span></span>|<span data-ttu-id="f204d-172">Остановка заданных тонов в конец записи.</span><span class="sxs-lookup"><span data-stu-id="f204d-172">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="f204d-173">Контекст</span><span class="sxs-lookup"><span data-stu-id="f204d-173">clientContext</span></span>|<span data-ttu-id="f204d-174">String</span><span class="sxs-lookup"><span data-stu-id="f204d-174">String</span></span>|<span data-ttu-id="f204d-175">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="f204d-175">Unique Client Context string.</span></span> <span data-ttu-id="f204d-176">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="f204d-176">Max limit is 256 chars.</span></span>|

> <span data-ttu-id="f204d-177">**Примечание:** Максимальное время записи сократилось с 5 минут до 2 минут.</span><span class="sxs-lookup"><span data-stu-id="f204d-177">**Note:** The maximum recording time has been reduced from 5 minutes to 2 minutes.</span></span>

## <a name="response"></a><span data-ttu-id="f204d-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="f204d-178">Response</span></span>
<span data-ttu-id="f204d-179">Этот метод возвращает `200 OK` код HTTP-ответа и заголовок Location с URI для [рекордоператион](../resources/recordoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="f204d-179">This method returns a `200 OK` HTTP response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="f204d-180">Пример</span><span class="sxs-lookup"><span data-stu-id="f204d-180">Example</span></span>
<span data-ttu-id="f204d-181">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f204d-181">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="f204d-182">Пример 1: записывает короткий звуковой ответ от вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="f204d-182">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="f204d-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="f204d-183">Request</span></span>
<span data-ttu-id="f204d-184">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f204d-184">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f204d-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="f204d-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-recordResponse"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/recordResponse
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
# <a name="javascript"></a>[<span data-ttu-id="f204d-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f204d-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f204d-187">C#</span><span class="sxs-lookup"><span data-stu-id="f204d-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f204d-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f204d-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f204d-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="f204d-189">Response</span></span>
<span data-ttu-id="f204d-190">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f204d-190">The following example shows the response.</span></span>

> <span data-ttu-id="f204d-p115">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f204d-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "completionReason": null,
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="f204d-193">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="f204d-193">Notification - operation completed</span></span>

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
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="f204d-194">Пример 2: получение файла записи</span><span class="sxs-lookup"><span data-stu-id="f204d-194">Example 2: Retrieving the recording file</span></span>

> <span data-ttu-id="f204d-195">**Примечание:** Вы не можете записать или оставить мультимедийный контент из звонков или собраний, к которым обращается приложение, или данных, полученных из этого контента.</span><span class="sxs-lookup"><span data-stu-id="f204d-195">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="f204d-196">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="f204d-196">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="f204d-197">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="f204d-197">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="f204d-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="f204d-198">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="f204d-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="f204d-199">Response</span></span>

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

> <span data-ttu-id="f204d-200">**Примечание:** Вы не можете записать или оставить мультимедийный контент из звонков или собраний, к которым обращается приложение, или данных, полученных из этого контента.</span><span class="sxs-lookup"><span data-stu-id="f204d-200">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="f204d-201">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="f204d-201">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="f204d-202">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="f204d-202">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: recordResponse",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


