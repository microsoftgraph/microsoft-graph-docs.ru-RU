---
title: 'Call: Рекордреспонсе'
description: Запись короткого голосового ответа звонящего. Это полезно, если пользователь-Робот хочет записать голосовой ответ от абонента, вызываемого после приглашения.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b3d6ec3bdaa8a2d9f9cc25d30a5e9250545eeb41
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023396"
---
# <a name="call-recordresponse"></a><span data-ttu-id="fbe7d-104">Call: Рекордреспонсе</span><span class="sxs-lookup"><span data-stu-id="fbe7d-104">call: recordResponse</span></span>

<span data-ttu-id="fbe7d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbe7d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fbe7d-106">Запись короткого голосового ответа звонящего.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-106">Records a short audio response from the caller.</span></span>
<span data-ttu-id="fbe7d-107">С помощью Bot можно получить голосовой ответ от вызывающего абонента после того, как им будет предложено ответить.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-107">A bot can utilize this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="fbe7d-108">Дополнительные сведения о том, как обрабатывать операции, смотрите в [коммсоператион](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="fbe7d-108">For further information on how to handle operations, please review [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="fbe7d-109">**Примечание:** Это поддерживается только для [вызовов](../resources/call.md) , которые инициируются с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="fbe7d-109">**Note:** This is only supported for [calls](../resources/call.md) which are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="fbe7d-110">Это действие не предназначено для записи всего вызова.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-110">This action is not intended to record the entire call.</span></span> <span data-ttu-id="fbe7d-111">Максимальная длина записи составляет 2 минуты.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-111">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="fbe7d-112">Запись не сохраняется окончательно при помощи платформы Cloud Communications и удаляется вскоре после завершения вызова.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-112">The recording is not saved permanently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="fbe7d-113">Bot должен сразу скачать запись после завершения операции записи, используя значение Рекординглокатион, указанное в завершенном уведомлении.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-113">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="fbe7d-114">**Примечание:** Собранные файлы мультимедиа могут быть **не** сохранены.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-114">**Note:** Any media collected may **not** be persisted.</span></span> <span data-ttu-id="fbe7d-115">Убедитесь, что вы соответствуете законам и нормативам вашей области, когда дело доходит до записи звонков.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-115">Make sure you are compliant with the laws and regulations of your area when it comes to call recording.</span></span> <span data-ttu-id="fbe7d-116">Для получения дополнительных сведений обратитесь в юридическое Юрисконсульта.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-116">Please consult with a legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbe7d-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbe7d-117">Permissions</span></span>
<span data-ttu-id="fbe7d-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbe7d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fbe7d-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbe7d-120">Permission type</span></span> | <span data-ttu-id="fbe7d-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbe7d-121">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="fbe7d-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbe7d-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="fbe7d-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fbe7d-123">Not Supported</span></span>        |
| <span data-ttu-id="fbe7d-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbe7d-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbe7d-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fbe7d-125">Not Supported</span></span>        |
| <span data-ttu-id="fbe7d-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbe7d-126">Application</span></span>     | <span data-ttu-id="fbe7d-127">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="fbe7d-127">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="fbe7d-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbe7d-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/recordResponse
```

## <a name="request-headers"></a><span data-ttu-id="fbe7d-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbe7d-129">Request headers</span></span>
| <span data-ttu-id="fbe7d-130">Имя</span><span class="sxs-lookup"><span data-stu-id="fbe7d-130">Name</span></span>          | <span data-ttu-id="fbe7d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fbe7d-131">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fbe7d-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbe7d-132">Authorization</span></span> | <span data-ttu-id="fbe7d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbe7d-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fbe7d-135">Request body</span></span>
<span data-ttu-id="fbe7d-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fbe7d-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="fbe7d-137">Parameter</span></span>      | <span data-ttu-id="fbe7d-138">Тип</span><span class="sxs-lookup"><span data-stu-id="fbe7d-138">Type</span></span>    |<span data-ttu-id="fbe7d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="fbe7d-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbe7d-140">выдан</span><span class="sxs-lookup"><span data-stu-id="fbe7d-140">prompts</span></span>|<span data-ttu-id="fbe7d-141">Коллекция [медиапромпт](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="fbe7d-141">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="fbe7d-142">Приглашения для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-142">The prompts to be played.</span></span> <span data-ttu-id="fbe7d-143">Максимальный поддерживаемый размер коллекции Медиапромпт составляет 1.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-143">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="fbe7d-144">баржеиналловед</span><span class="sxs-lookup"><span data-stu-id="fbe7d-144">bargeInAllowed</span></span>|<span data-ttu-id="fbe7d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbe7d-145">Boolean</span></span>| <span data-ttu-id="fbe7d-146">Если этот параметр имеет значение true, запрос Рекордреспонсе будет барже в другие существующие запросы записи или плайпромпт в очереди.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-146">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="fbe7d-147">Значение по умолчанию = false.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-147">Default = false.</span></span> |
|<span data-ttu-id="fbe7d-148">инитиалсиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="fbe7d-148">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="fbe7d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fbe7d-149">Int32</span></span>| <span data-ttu-id="fbe7d-150">Максимальное значение параметра "тишина" (тишина пользователя) разрешено с момента запуска операции записи ответа до истечения времени ожидания и сбоев операции.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-150">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="fbe7d-151">При воспроизведении приглашения этот таймер запускается после завершения приглашения.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-151">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="fbe7d-152">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд</span><span class="sxs-lookup"><span data-stu-id="fbe7d-152">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="fbe7d-153">макссиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="fbe7d-153">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="fbe7d-154">Int32</span><span class="sxs-lookup"><span data-stu-id="fbe7d-154">Int32</span></span>| <span data-ttu-id="fbe7d-155">Максимально допустимое время тишины (пауза) после начала диктовки пользователя.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-155">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="fbe7d-156">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-156">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="fbe7d-157">максрекорддуратионинсекондс</span><span class="sxs-lookup"><span data-stu-id="fbe7d-157">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="fbe7d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fbe7d-158">Int32</span></span>| <span data-ttu-id="fbe7d-159">Максимальная длительность операции Рекордреспонсе перед остановкой записи.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-159">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="fbe7d-160">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-160">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="fbe7d-161">плайбип</span><span class="sxs-lookup"><span data-stu-id="fbe7d-161">playBeep</span></span>|<span data-ttu-id="fbe7d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbe7d-162">Boolean</span></span>| <span data-ttu-id="fbe7d-163">Если этот параметр имеет значение true, воспроизводит звуковой сигнал, указывающий пользователю, что он может начать запись сообщения.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-163">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="fbe7d-164">Значение по умолчанию = true.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-164">Default = true.</span></span>|
|<span data-ttu-id="fbe7d-165">стоптонес</span><span class="sxs-lookup"><span data-stu-id="fbe7d-165">stopTones</span></span>|<span data-ttu-id="fbe7d-166">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fbe7d-166">String collection</span></span>|<span data-ttu-id="fbe7d-167">Остановка заданных тонов в конец записи.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-167">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="fbe7d-168">Контекст</span><span class="sxs-lookup"><span data-stu-id="fbe7d-168">clientContext</span></span>|<span data-ttu-id="fbe7d-169">String</span><span class="sxs-lookup"><span data-stu-id="fbe7d-169">String</span></span>|<span data-ttu-id="fbe7d-170">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-170">Unique Client Context string.</span></span> <span data-ttu-id="fbe7d-171">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-171">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="fbe7d-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbe7d-172">Response</span></span>
<span data-ttu-id="fbe7d-173">Этот метод возвращает `200 OK` код отклика и заголовок Location с URI для [рекордоператион](../resources/recordoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-173">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="fbe7d-174">Пример</span><span class="sxs-lookup"><span data-stu-id="fbe7d-174">Example</span></span>
<span data-ttu-id="fbe7d-175">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-175">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="fbe7d-176">Пример 1: записывает короткий звуковой ответ от вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-176">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="fbe7d-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbe7d-177">Request</span></span>
<span data-ttu-id="fbe7d-178">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-178">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fbe7d-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbe7d-179">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fbe7d-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbe7d-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fbe7d-181">C#</span><span class="sxs-lookup"><span data-stu-id="fbe7d-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbe7d-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbe7d-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fbe7d-183">Java</span><span class="sxs-lookup"><span data-stu-id="fbe7d-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-recordresponse-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fbe7d-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbe7d-184">Response</span></span>
<span data-ttu-id="fbe7d-185">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-185">The following example shows the response.</span></span>

> <span data-ttu-id="fbe7d-p114">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="fbe7d-188">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="fbe7d-188">Notification - operation completed</span></span>

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

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="fbe7d-189">Пример 2: получение файла записи</span><span class="sxs-lookup"><span data-stu-id="fbe7d-189">Example 2: Retrieving the recording file</span></span>

><span data-ttu-id="fbe7d-190">**Примечание:** Вы не можете записать или оставить мультимедийный контент из звонков или собраний, к которым обращается приложение, или данных, полученных из этого контента.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-190">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="fbe7d-191">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-191">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="fbe7d-192">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="fbe7d-192">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="fbe7d-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbe7d-193">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="fbe7d-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbe7d-194">Response</span></span>

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

