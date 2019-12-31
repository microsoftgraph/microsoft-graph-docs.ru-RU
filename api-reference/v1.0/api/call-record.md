---
title: 'Call: Рекордреспонсе'
description: Запись короткого голосового ответа звонящего. Это полезно, если пользователь-Робот хочет записать голосовой ответ от абонента, вызываемого после приглашения.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 530cab8a11344959df32f7acc41bb706162ccab1
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913263"
---
# <a name="call-recordresponse"></a><span data-ttu-id="80efe-104">Call: Рекордреспонсе</span><span class="sxs-lookup"><span data-stu-id="80efe-104">call: recordResponse</span></span>

<span data-ttu-id="80efe-105">Запись короткого голосового ответа звонящего.</span><span class="sxs-lookup"><span data-stu-id="80efe-105">Records a short audio response from the caller.</span></span>
<span data-ttu-id="80efe-106">С помощью Bot можно получить голосовой ответ от вызывающего абонента после того, как им будет предложено ответить.</span><span class="sxs-lookup"><span data-stu-id="80efe-106">A bot can utilize this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="80efe-107">Дополнительные сведения о том, как обрабатывать операции, смотрите в [коммсоператион](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="80efe-107">For further information on how to handle operations, please review [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="80efe-108">**Примечание:** Это поддерживается только для [вызовов](../resources/call.md) , которые инициируются с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="80efe-108">**Note:** This is only supported for [calls](../resources/call.md) which are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="80efe-109">Это действие не предназначено для записи всего вызова.</span><span class="sxs-lookup"><span data-stu-id="80efe-109">This action is not intended to record the entire call.</span></span> <span data-ttu-id="80efe-110">Максимальная длина записи составляет 2 минуты.</span><span class="sxs-lookup"><span data-stu-id="80efe-110">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="80efe-111">Запись не сохраняется окончательно при помощи платформы Cloud Communications и удаляется вскоре после завершения вызова.</span><span class="sxs-lookup"><span data-stu-id="80efe-111">The recording is not saved permanently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="80efe-112">Bot должен сразу скачать запись после завершения операции записи, используя значение Рекординглокатион, указанное в завершенном уведомлении.</span><span class="sxs-lookup"><span data-stu-id="80efe-112">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="80efe-113">**Примечание:** Собранные файлы мультимедиа могут быть **не** сохранены.</span><span class="sxs-lookup"><span data-stu-id="80efe-113">**Note:** Any media collected may **not** be persisted.</span></span> <span data-ttu-id="80efe-114">Убедитесь, что вы соответствуете законам и нормативам вашей области, когда дело доходит до записи звонков.</span><span class="sxs-lookup"><span data-stu-id="80efe-114">Make sure you are compliant with the laws and regulations of your area when it comes to call recording.</span></span> <span data-ttu-id="80efe-115">Для получения дополнительных сведений обратитесь в юридическое Юрисконсульта.</span><span class="sxs-lookup"><span data-stu-id="80efe-115">Please consult with a legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="80efe-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80efe-116">Permissions</span></span>
<span data-ttu-id="80efe-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80efe-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80efe-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80efe-119">Permission type</span></span> | <span data-ttu-id="80efe-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80efe-120">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="80efe-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80efe-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="80efe-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="80efe-122">Not Supported</span></span>        |
| <span data-ttu-id="80efe-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80efe-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80efe-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="80efe-124">Not Supported</span></span>        |
| <span data-ttu-id="80efe-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80efe-125">Application</span></span>     | <span data-ttu-id="80efe-126">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="80efe-126">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="80efe-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80efe-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/recordResponse
```

## <a name="request-headers"></a><span data-ttu-id="80efe-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80efe-128">Request headers</span></span>
| <span data-ttu-id="80efe-129">Имя</span><span class="sxs-lookup"><span data-stu-id="80efe-129">Name</span></span>          | <span data-ttu-id="80efe-130">Описание</span><span class="sxs-lookup"><span data-stu-id="80efe-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="80efe-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80efe-131">Authorization</span></span> | <span data-ttu-id="80efe-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80efe-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80efe-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80efe-134">Request body</span></span>
<span data-ttu-id="80efe-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="80efe-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="80efe-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="80efe-136">Parameter</span></span>      | <span data-ttu-id="80efe-137">Тип</span><span class="sxs-lookup"><span data-stu-id="80efe-137">Type</span></span>    |<span data-ttu-id="80efe-138">Описание</span><span class="sxs-lookup"><span data-stu-id="80efe-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80efe-139">выдан</span><span class="sxs-lookup"><span data-stu-id="80efe-139">prompts</span></span>|<span data-ttu-id="80efe-140">Коллекция [медиапромпт](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="80efe-140">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="80efe-141">Приглашения для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="80efe-141">The prompts to be played.</span></span> <span data-ttu-id="80efe-142">Максимальный поддерживаемый размер коллекции Медиапромпт составляет 1.</span><span class="sxs-lookup"><span data-stu-id="80efe-142">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="80efe-143">баржеиналловед</span><span class="sxs-lookup"><span data-stu-id="80efe-143">bargeInAllowed</span></span>|<span data-ttu-id="80efe-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="80efe-144">Boolean</span></span>| <span data-ttu-id="80efe-145">Если этот параметр имеет значение true, запрос Рекордреспонсе будет барже в другие существующие запросы записи или плайпромпт в очереди.</span><span class="sxs-lookup"><span data-stu-id="80efe-145">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="80efe-146">Значение по умолчанию = false.</span><span class="sxs-lookup"><span data-stu-id="80efe-146">Default = false.</span></span> |
|<span data-ttu-id="80efe-147">инитиалсиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="80efe-147">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="80efe-148">Int32</span><span class="sxs-lookup"><span data-stu-id="80efe-148">Int32</span></span>| <span data-ttu-id="80efe-149">Максимальное значение параметра "тишина" (тишина пользователя) разрешено с момента запуска операции записи ответа до истечения времени ожидания и сбоев операции.</span><span class="sxs-lookup"><span data-stu-id="80efe-149">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="80efe-150">При воспроизведении приглашения этот таймер запускается после завершения приглашения.</span><span class="sxs-lookup"><span data-stu-id="80efe-150">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="80efe-151">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд</span><span class="sxs-lookup"><span data-stu-id="80efe-151">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="80efe-152">макссиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="80efe-152">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="80efe-153">Int32</span><span class="sxs-lookup"><span data-stu-id="80efe-153">Int32</span></span>| <span data-ttu-id="80efe-154">Максимально допустимое время тишины (пауза) после начала диктовки пользователя.</span><span class="sxs-lookup"><span data-stu-id="80efe-154">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="80efe-155">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="80efe-155">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="80efe-156">максрекорддуратионинсекондс</span><span class="sxs-lookup"><span data-stu-id="80efe-156">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="80efe-157">Int32</span><span class="sxs-lookup"><span data-stu-id="80efe-157">Int32</span></span>| <span data-ttu-id="80efe-158">Максимальная длительность операции Рекордреспонсе перед остановкой записи.</span><span class="sxs-lookup"><span data-stu-id="80efe-158">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="80efe-159">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 120 секунд.</span><span class="sxs-lookup"><span data-stu-id="80efe-159">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="80efe-160">плайбип</span><span class="sxs-lookup"><span data-stu-id="80efe-160">playBeep</span></span>|<span data-ttu-id="80efe-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="80efe-161">Boolean</span></span>| <span data-ttu-id="80efe-162">Если этот параметр имеет значение true, воспроизводит звуковой сигнал, указывающий пользователю, что он может начать запись сообщения.</span><span class="sxs-lookup"><span data-stu-id="80efe-162">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="80efe-163">Значение по умолчанию = true.</span><span class="sxs-lookup"><span data-stu-id="80efe-163">Default = true.</span></span>|
|<span data-ttu-id="80efe-164">стоптонес</span><span class="sxs-lookup"><span data-stu-id="80efe-164">stopTones</span></span>|<span data-ttu-id="80efe-165">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="80efe-165">String collection</span></span>|<span data-ttu-id="80efe-166">Остановка заданных тонов в конец записи.</span><span class="sxs-lookup"><span data-stu-id="80efe-166">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="80efe-167">Контекст</span><span class="sxs-lookup"><span data-stu-id="80efe-167">clientContext</span></span>|<span data-ttu-id="80efe-168">String</span><span class="sxs-lookup"><span data-stu-id="80efe-168">String</span></span>|<span data-ttu-id="80efe-169">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="80efe-169">Unique Client Context string.</span></span> <span data-ttu-id="80efe-170">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="80efe-170">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="80efe-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="80efe-171">Response</span></span>
<span data-ttu-id="80efe-172">Этот метод возвращает код `200 OK` отклика и заголовок Location с URI для [рекордоператион](../resources/recordoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="80efe-172">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="80efe-173">Пример</span><span class="sxs-lookup"><span data-stu-id="80efe-173">Example</span></span>
<span data-ttu-id="80efe-174">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="80efe-174">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="80efe-175">Пример 1: записывает короткий звуковой ответ от вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="80efe-175">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="80efe-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="80efe-176">Request</span></span>
<span data-ttu-id="80efe-177">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80efe-177">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="80efe-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="80efe-178">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80efe-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80efe-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="80efe-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="80efe-180">Response</span></span>
<span data-ttu-id="80efe-181">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="80efe-181">The following example shows the response.</span></span>

> <span data-ttu-id="80efe-p114">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80efe-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="80efe-184">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="80efe-184">Notification - operation completed</span></span>

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

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="80efe-185">Пример 2: получение файла записи</span><span class="sxs-lookup"><span data-stu-id="80efe-185">Example 2: Retrieving the recording file</span></span>

><span data-ttu-id="80efe-186">**Примечание:** Вы не можете записать или оставить мультимедийный контент из звонков или собраний, к которым обращается приложение, или данных, полученных из этого контента.</span><span class="sxs-lookup"><span data-stu-id="80efe-186">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="80efe-187">Убедитесь, что вы соответствуете законам и нормативам, касающимся защиты данных и конфиденциальности коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="80efe-187">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="80efe-188">Дополнительные сведения можно узнать из [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) и обратившись за юридической помощью.</span><span class="sxs-lookup"><span data-stu-id="80efe-188">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="80efe-189">Запросить</span><span class="sxs-lookup"><span data-stu-id="80efe-189">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="80efe-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="80efe-190">Response</span></span>

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
