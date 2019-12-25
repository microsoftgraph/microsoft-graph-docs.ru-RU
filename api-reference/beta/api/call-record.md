---
title: 'Call: Рекордреспонсе'
description: Запишите короткий звуковой ответ от вызывающего абонента. Это полезно, если Bot хочет записать голосовой ответ от абонента, вызываемого после приглашения.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fac72a4f0436980fd143d9a9011a6bd73c2c3c76
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868263"
---
# <a name="call-recordresponse"></a><span data-ttu-id="375a7-104">Call: Рекордреспонсе</span><span class="sxs-lookup"><span data-stu-id="375a7-104">call: recordResponse</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="375a7-105">Запишите короткий звуковой ответ от вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="375a7-105">Record a short audio response from the caller.</span></span>

<span data-ttu-id="375a7-106">С помощью Bot можно получить голосовой ответ от вызывающего абонента после получения запроса на ответ.</span><span class="sxs-lookup"><span data-stu-id="375a7-106">A bot can use this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="375a7-107">Дополнительные сведения об обработке операций можно найти в статье [коммсоператион](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="375a7-107">For more information about how to handle operations, see [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="375a7-108">**Примечание:** Этот API поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="375a7-108">**Note:** This API is only supported for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="375a7-109">Это действие не предназначено для записи всего вызова.</span><span class="sxs-lookup"><span data-stu-id="375a7-109">This action is not intended to record the entire call.</span></span> <span data-ttu-id="375a7-110">Максимальная длина записи составляет 2 минуты.</span><span class="sxs-lookup"><span data-stu-id="375a7-110">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="375a7-111">Запись не сохраняется окончательно при помощи платформы Cloud Communications и удаляется вскоре после завершения вызова.</span><span class="sxs-lookup"><span data-stu-id="375a7-111">The recording is not saved permanently by the by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="375a7-112">Bot должен сразу скачать запись после завершения операции записи, используя значение Рекординглокатион, указанное в завершенном уведомлении.</span><span class="sxs-lookup"><span data-stu-id="375a7-112">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="375a7-113">**Примечание:** Вы не можете записать или оставить мультимедийный контент из звонков или собраний, к которым обращается приложение, или данных, полученных из этого контента.</span><span class="sxs-lookup"><span data-stu-id="375a7-113">**Note:** You may not record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="375a7-114">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="375a7-114">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="375a7-115">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="375a7-115">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="375a7-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="375a7-116">Permissions</span></span>
<span data-ttu-id="375a7-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="375a7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="375a7-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="375a7-119">Permission type</span></span> | <span data-ttu-id="375a7-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="375a7-120">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="375a7-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="375a7-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="375a7-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="375a7-122">Not Supported</span></span>        |
| <span data-ttu-id="375a7-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="375a7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="375a7-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="375a7-124">Not Supported</span></span>        |
| <span data-ttu-id="375a7-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="375a7-125">Application</span></span>     | <span data-ttu-id="375a7-126">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="375a7-126">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="375a7-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="375a7-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/recordResponse
POST /communications/calls/{id}/recordResponse
```
> <span data-ttu-id="375a7-128">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="375a7-128">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="375a7-129">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="375a7-129">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="375a7-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="375a7-130">Request headers</span></span>
| <span data-ttu-id="375a7-131">Имя</span><span class="sxs-lookup"><span data-stu-id="375a7-131">Name</span></span>          | <span data-ttu-id="375a7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="375a7-132">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="375a7-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="375a7-133">Authorization</span></span> | <span data-ttu-id="375a7-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="375a7-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="375a7-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="375a7-136">Content-type</span></span>| <span data-ttu-id="375a7-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="375a7-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="375a7-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="375a7-139">Request body</span></span>
<span data-ttu-id="375a7-140">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="375a7-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="375a7-141">Параметр</span><span class="sxs-lookup"><span data-stu-id="375a7-141">Parameter</span></span>      | <span data-ttu-id="375a7-142">Тип</span><span class="sxs-lookup"><span data-stu-id="375a7-142">Type</span></span>    |<span data-ttu-id="375a7-143">Описание</span><span class="sxs-lookup"><span data-stu-id="375a7-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="375a7-144">выдан</span><span class="sxs-lookup"><span data-stu-id="375a7-144">prompts</span></span>|<span data-ttu-id="375a7-145">Коллекция [медиапромпт](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="375a7-145">[MediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="375a7-146">Приглашения для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="375a7-146">The prompts to be played.</span></span> <span data-ttu-id="375a7-147">Максимальный поддерживаемый размер коллекции Медиапромпт составляет 1.</span><span class="sxs-lookup"><span data-stu-id="375a7-147">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="375a7-148">баржеиналловед</span><span class="sxs-lookup"><span data-stu-id="375a7-148">bargeInAllowed</span></span>|<span data-ttu-id="375a7-149">Логический</span><span class="sxs-lookup"><span data-stu-id="375a7-149">Boolean</span></span>| <span data-ttu-id="375a7-150">Если этот параметр имеет значение true, запрос Рекордреспонсе будет барже в другие существующие запросы записи или плайпромпт в очереди.</span><span class="sxs-lookup"><span data-stu-id="375a7-150">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="375a7-151">Значение по умолчанию = false.</span><span class="sxs-lookup"><span data-stu-id="375a7-151">Default = false.</span></span> |
|<span data-ttu-id="375a7-152">инитиалсиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="375a7-152">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="375a7-153">Int32</span><span class="sxs-lookup"><span data-stu-id="375a7-153">Int32</span></span>| <span data-ttu-id="375a7-154">Максимальное значение параметра "тишина" (тишина пользователя) разрешено с момента запуска операции записи ответа до истечения времени ожидания и сбоев операции.</span><span class="sxs-lookup"><span data-stu-id="375a7-154">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="375a7-155">При воспроизведении приглашения этот таймер запускается после завершения приглашения.</span><span class="sxs-lookup"><span data-stu-id="375a7-155">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="375a7-156">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд</span><span class="sxs-lookup"><span data-stu-id="375a7-156">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="375a7-157">макссиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="375a7-157">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="375a7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="375a7-158">Int32</span></span>| <span data-ttu-id="375a7-159">Максимально допустимое время тишины (пауза) после начала диктовки пользователя.</span><span class="sxs-lookup"><span data-stu-id="375a7-159">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="375a7-160">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="375a7-160">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="375a7-161">максрекорддуратионинсекондс</span><span class="sxs-lookup"><span data-stu-id="375a7-161">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="375a7-162">Int32</span><span class="sxs-lookup"><span data-stu-id="375a7-162">Int32</span></span>| <span data-ttu-id="375a7-163">Максимальная длительность операции Рекордреспонсе перед остановкой записи.</span><span class="sxs-lookup"><span data-stu-id="375a7-163">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="375a7-164">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="375a7-164">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="375a7-165">плайбип</span><span class="sxs-lookup"><span data-stu-id="375a7-165">playBeep</span></span>|<span data-ttu-id="375a7-166">Логический</span><span class="sxs-lookup"><span data-stu-id="375a7-166">Boolean</span></span>| <span data-ttu-id="375a7-167">Если этот параметр имеет значение true, воспроизводит звуковой сигнал, указывающий пользователю, что он может начать запись сообщения.</span><span class="sxs-lookup"><span data-stu-id="375a7-167">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="375a7-168">Значение по умолчанию = true.</span><span class="sxs-lookup"><span data-stu-id="375a7-168">Default = true.</span></span>|
|<span data-ttu-id="375a7-169">стоптонес</span><span class="sxs-lookup"><span data-stu-id="375a7-169">stopTones</span></span>|<span data-ttu-id="375a7-170">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="375a7-170">String collection</span></span>|<span data-ttu-id="375a7-171">Остановка заданных тонов в конец записи.</span><span class="sxs-lookup"><span data-stu-id="375a7-171">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="375a7-172">Контекст</span><span class="sxs-lookup"><span data-stu-id="375a7-172">clientContext</span></span>|<span data-ttu-id="375a7-173">String</span><span class="sxs-lookup"><span data-stu-id="375a7-173">String</span></span>|<span data-ttu-id="375a7-174">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="375a7-174">Unique Client Context string.</span></span> <span data-ttu-id="375a7-175">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="375a7-175">Max limit is 256 chars.</span></span>|

> <span data-ttu-id="375a7-176">**Примечание:** Максимальное время записи сократилось с 5 минут до 2 минут.</span><span class="sxs-lookup"><span data-stu-id="375a7-176">**Note:** The maximum recording time has been reduced from 5 minutes to 2 minutes.</span></span>

## <a name="response"></a><span data-ttu-id="375a7-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="375a7-177">Response</span></span>
<span data-ttu-id="375a7-178">Этот метод возвращает код `200 OK` HTTP-ответа и заголовок Location с URI для [рекордоператион](../resources/recordoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="375a7-178">This method returns a `200 OK` HTTP response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="375a7-179">Пример</span><span class="sxs-lookup"><span data-stu-id="375a7-179">Example</span></span>
<span data-ttu-id="375a7-180">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="375a7-180">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="375a7-181">Пример 1: записывает короткий звуковой ответ от вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="375a7-181">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="375a7-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="375a7-182">Request</span></span>
<span data-ttu-id="375a7-183">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="375a7-183">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="375a7-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="375a7-184">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="375a7-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="375a7-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="375a7-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="375a7-186">Response</span></span>
<span data-ttu-id="375a7-187">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="375a7-187">The following example shows the response.</span></span>

> <span data-ttu-id="375a7-p115">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="375a7-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="375a7-190">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="375a7-190">Notification - operation completed</span></span>

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

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="375a7-191">Пример 2: получение файла записи</span><span class="sxs-lookup"><span data-stu-id="375a7-191">Example 2: Retrieving the recording file</span></span>

> <span data-ttu-id="375a7-192">**Примечание:** Вы не можете записать или оставить мультимедийный контент из звонков или собраний, к которым обращается приложение, или данных, полученных из этого контента.</span><span class="sxs-lookup"><span data-stu-id="375a7-192">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="375a7-193">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="375a7-193">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="375a7-194">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="375a7-194">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="375a7-195">Запросить</span><span class="sxs-lookup"><span data-stu-id="375a7-195">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="375a7-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="375a7-196">Response</span></span>

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

> <span data-ttu-id="375a7-197">**Примечание:** Вы не можете записать или оставить мультимедийный контент из звонков или собраний, к которым обращается приложение, или данных, полученных из этого контента.</span><span class="sxs-lookup"><span data-stu-id="375a7-197">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="375a7-198">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="375a7-198">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="375a7-199">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="375a7-199">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

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
