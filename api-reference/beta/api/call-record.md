---
title: 'Call: Record'
description: Запись короткого аудиоклипа из вызова. Это полезно, если пользователь-Робот хочет записать голосовой ответ от абонента, вызываемого после приглашения.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2961bacfa9092aa580801e42e44aa1d2adbfaa97
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636703"
---
# <a name="call-record"></a><span data-ttu-id="f76bc-104">Call: Record</span><span class="sxs-lookup"><span data-stu-id="f76bc-104">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f76bc-105">Запись короткого аудиоклипа из вызова.</span><span class="sxs-lookup"><span data-stu-id="f76bc-105">Record a short audio clip from a call.</span></span>
<span data-ttu-id="f76bc-106">С помощью Bot можно получить голосовой ответ от вызывающего абонента после того, как им будет предложено ответить.</span><span class="sxs-lookup"><span data-stu-id="f76bc-106">A bot can utilize this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="f76bc-107">Дополнительные сведения о том, как обрабатывать операции, смотрите в [коммсоператион](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="f76bc-107">For further information on how to handle operations, please review [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="f76bc-108">**Примечание:** Это поддерживается только для [вызовов](../resources/call.md) , которые инициируются с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="f76bc-108">**Note:** This is only supported for [calls](../resources/call.md) which are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="f76bc-109">Это действие не предназначено для записи всего вызова.</span><span class="sxs-lookup"><span data-stu-id="f76bc-109">This action is not intended to record the entire call.</span></span> <span data-ttu-id="f76bc-110">Максимальная длина записи составляет 5 минут.</span><span class="sxs-lookup"><span data-stu-id="f76bc-110">The maximum length of recording is 5 minutes.</span></span> <span data-ttu-id="f76bc-111">Запись не сохраняется окончательно при помощи платформы Cloud Communications и удаляется вскоре после завершения вызова.</span><span class="sxs-lookup"><span data-stu-id="f76bc-111">The recording is not saved permanently by the by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="f76bc-112">Bot должен сразу скачать запись после завершения операции записи, используя значение Рекординглокатион, указанное в завершенном уведомлении.</span><span class="sxs-lookup"><span data-stu-id="f76bc-112">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="f76bc-113">**Примечание:** Собранные файлы мультимедиа могут быть **не** сохранены.</span><span class="sxs-lookup"><span data-stu-id="f76bc-113">**Note:** Any media collected may **not** be persisted.</span></span> <span data-ttu-id="f76bc-114">Убедитесь, что вы соответствуете законам и нормативам вашей области, когда дело доходит до записи звонков.</span><span class="sxs-lookup"><span data-stu-id="f76bc-114">Make sure you are compliant with the laws and regulations of your area when it comes to call recording.</span></span> <span data-ttu-id="f76bc-115">Для получения дополнительных сведений обратитесь в юридическое Юрисконсульта.</span><span class="sxs-lookup"><span data-stu-id="f76bc-115">Please consult with a legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="f76bc-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f76bc-116">Permissions</span></span>
<span data-ttu-id="f76bc-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f76bc-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f76bc-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f76bc-119">Permission type</span></span> | <span data-ttu-id="f76bc-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f76bc-120">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="f76bc-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f76bc-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="f76bc-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f76bc-122">Not Supported</span></span>        |
| <span data-ttu-id="f76bc-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f76bc-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f76bc-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f76bc-124">Not Supported</span></span>        |
| <span data-ttu-id="f76bc-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="f76bc-125">Application</span></span>     | <span data-ttu-id="f76bc-126">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="f76bc-126">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="f76bc-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f76bc-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /communications/calls/{id}/record
```
> <span data-ttu-id="f76bc-128">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="f76bc-128">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="f76bc-129">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="f76bc-129">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f76bc-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f76bc-130">Request headers</span></span>
| <span data-ttu-id="f76bc-131">Имя</span><span class="sxs-lookup"><span data-stu-id="f76bc-131">Name</span></span>          | <span data-ttu-id="f76bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f76bc-132">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f76bc-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f76bc-133">Authorization</span></span> | <span data-ttu-id="f76bc-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f76bc-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f76bc-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f76bc-136">Request body</span></span>
<span data-ttu-id="f76bc-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f76bc-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f76bc-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="f76bc-138">Parameter</span></span>      | <span data-ttu-id="f76bc-139">Тип</span><span class="sxs-lookup"><span data-stu-id="f76bc-139">Type</span></span>    |<span data-ttu-id="f76bc-140">Описание</span><span class="sxs-lookup"><span data-stu-id="f76bc-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f76bc-141">выдан</span><span class="sxs-lookup"><span data-stu-id="f76bc-141">prompts</span></span>|<span data-ttu-id="f76bc-142">Коллекция [медиапромпт](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="f76bc-142">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="f76bc-143">Коллекция приглашений для воспроизведения (при наличии) до начала записи.</span><span class="sxs-lookup"><span data-stu-id="f76bc-143">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="f76bc-144">Пользователи могут указать действие "Плайпромпт" отдельно или указать его как часть "запись", в основном все записи прецеедед по приглашению.</span><span class="sxs-lookup"><span data-stu-id="f76bc-144">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt.</span></span> <span data-ttu-id="f76bc-145">Текущая поддержка предназначена только для одного приглашения в коллекции.</span><span class="sxs-lookup"><span data-stu-id="f76bc-145">Current support is only for a single prompt as part of the collection.</span></span> |
|<span data-ttu-id="f76bc-146">баржеиналловед</span><span class="sxs-lookup"><span data-stu-id="f76bc-146">bargeInAllowed</span></span>|<span data-ttu-id="f76bc-147">Логический</span><span class="sxs-lookup"><span data-stu-id="f76bc-147">Boolean</span></span>| <span data-ttu-id="f76bc-148">Если задано значение true, этот запрос будет барже в другие существующие запросы записи и плайпромпт, находящиеся в очереди.</span><span class="sxs-lookup"><span data-stu-id="f76bc-148">If true, this record request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="f76bc-149">Значение по умолчанию = false.</span><span class="sxs-lookup"><span data-stu-id="f76bc-149">Default = false.</span></span> |
|<span data-ttu-id="f76bc-150">инитиалсиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="f76bc-150">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="f76bc-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f76bc-151">Int32</span></span>| <span data-ttu-id="f76bc-152">Максимальное время ожидания (тишины пользователя), разрешенное с момента запуска операции записи до истечения времени ожидания и неудачи операции.</span><span class="sxs-lookup"><span data-stu-id="f76bc-152">Maximum initial silence (user silence) allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="f76bc-153">При воспроизведении приглашения этот таймер запускается после завершения приглашения.</span><span class="sxs-lookup"><span data-stu-id="f76bc-153">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="f76bc-154">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 300 секунд</span><span class="sxs-lookup"><span data-stu-id="f76bc-154">Default = 5 seconds, Min = 1 second, Max = 300 seconds</span></span> |
|<span data-ttu-id="f76bc-155">макссиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="f76bc-155">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="f76bc-156">Int32</span><span class="sxs-lookup"><span data-stu-id="f76bc-156">Int32</span></span>| <span data-ttu-id="f76bc-157">Максимально допустимое время тишины (пауза) после начала диктовки пользователя.</span><span class="sxs-lookup"><span data-stu-id="f76bc-157">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="f76bc-158">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 300 секунд.</span><span class="sxs-lookup"><span data-stu-id="f76bc-158">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="f76bc-159">максрекорддуратионинсекондс</span><span class="sxs-lookup"><span data-stu-id="f76bc-159">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="f76bc-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f76bc-160">Int32</span></span>| <span data-ttu-id="f76bc-161">Максимальная длительность операции записи перед остановкой записи.</span><span class="sxs-lookup"><span data-stu-id="f76bc-161">Max duration for a record operation before stopping recording.</span></span> <span data-ttu-id="f76bc-162">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 300 секунд.</span><span class="sxs-lookup"><span data-stu-id="f76bc-162">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="f76bc-163">плайбип</span><span class="sxs-lookup"><span data-stu-id="f76bc-163">playBeep</span></span>|<span data-ttu-id="f76bc-164">Логический</span><span class="sxs-lookup"><span data-stu-id="f76bc-164">Boolean</span></span>| <span data-ttu-id="f76bc-165">Если этот параметр имеет значение true, воспроизводит звуковой сигнал, указывающий пользователю, что он может начать запись сообщения.</span><span class="sxs-lookup"><span data-stu-id="f76bc-165">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="f76bc-166">Значение по умолчанию = true.</span><span class="sxs-lookup"><span data-stu-id="f76bc-166">Default = true.</span></span>|
|<span data-ttu-id="f76bc-167">стоптонес</span><span class="sxs-lookup"><span data-stu-id="f76bc-167">stopTones</span></span>|<span data-ttu-id="f76bc-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f76bc-168">String collection</span></span>|<span data-ttu-id="f76bc-169">Остановка заданных тонов в конец записи.</span><span class="sxs-lookup"><span data-stu-id="f76bc-169">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="f76bc-170">Контекст</span><span class="sxs-lookup"><span data-stu-id="f76bc-170">clientContext</span></span>|<span data-ttu-id="f76bc-171">String</span><span class="sxs-lookup"><span data-stu-id="f76bc-171">String</span></span>|<span data-ttu-id="f76bc-172">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="f76bc-172">Unique Client Context string.</span></span> <span data-ttu-id="f76bc-173">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="f76bc-173">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="f76bc-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f76bc-174">Response</span></span>
<span data-ttu-id="f76bc-175">Этот метод возвращает код `200 OK` отклика и заголовок Location с URI для [рекордоператион](../resources/recordoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="f76bc-175">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="f76bc-176">Пример</span><span class="sxs-lookup"><span data-stu-id="f76bc-176">Example</span></span>
<span data-ttu-id="f76bc-177">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f76bc-177">The following example shows how to call this API.</span></span>

### <a name="example-1-record-a-short-audio-clip-from-a-call"></a><span data-ttu-id="f76bc-178">Пример 1: запись короткого аудиоклипа из вызова</span><span class="sxs-lookup"><span data-stu-id="f76bc-178">Example 1: Record a short audio clip from a call</span></span>

##### <a name="request"></a><span data-ttu-id="f76bc-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="f76bc-179">Request</span></span>
<span data-ttu-id="f76bc-180">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f76bc-180">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f76bc-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="f76bc-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/record
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f76bc-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f76bc-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f76bc-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="f76bc-183">Response</span></span>
<span data-ttu-id="f76bc-184">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f76bc-184">The following example shows the response.</span></span>

> <span data-ttu-id="f76bc-p115">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f76bc-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="f76bc-187">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="f76bc-187">Notification - operation completed</span></span>

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

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="f76bc-188">Пример 2: получение файла записи</span><span class="sxs-lookup"><span data-stu-id="f76bc-188">Example 2: Retrieving the recording file</span></span>

> <span data-ttu-id="f76bc-189">**Примечание:** Несмотря на то, что вы можете получить и обработать запись, **необходимо** удалить ее позже.</span><span class="sxs-lookup"><span data-stu-id="f76bc-189">**Note:** While you're able to fetch the recording and process it, you **must** delete it afterwards.</span></span> <span data-ttu-id="f76bc-190">Невозможно оставить носитель.</span><span class="sxs-lookup"><span data-stu-id="f76bc-190">Media cannot be persisted.</span></span>

##### <a name="request"></a><span data-ttu-id="f76bc-191">Запросить</span><span class="sxs-lookup"><span data-stu-id="f76bc-191">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="f76bc-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="f76bc-192">Response</span></span>

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
