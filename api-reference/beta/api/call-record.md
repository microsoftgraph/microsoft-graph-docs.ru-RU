---
title: 'Call: Record'
description: Запись вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 473816bb52d441b4111632a69d767319ff59a17e
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062014"
---
# <a name="call-record"></a><span data-ttu-id="00418-103">Call: Record</span><span class="sxs-lookup"><span data-stu-id="00418-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00418-104">Запись короткого аудиоклипа из вызова.</span><span class="sxs-lookup"><span data-stu-id="00418-104">Record a short audio clip from the call.</span></span> <span data-ttu-id="00418-105">Это полезно, если Bot хочет записать голосовой ответ от абонента, вызываемого после приглашения.</span><span class="sxs-lookup"><span data-stu-id="00418-105">This is useful if the bot wants to capture a voice response from the caller following a prompt.</span></span>

> [!Note]
> <span data-ttu-id="00418-106">Действие записи поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="00418-106">The record action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span> <span data-ttu-id="00418-107">Это действие не записывает весь вызов.</span><span class="sxs-lookup"><span data-stu-id="00418-107">This action does not record the entire call.</span></span> <span data-ttu-id="00418-108">Максимальная длина записи составляет 5 минут.</span><span class="sxs-lookup"><span data-stu-id="00418-108">The maximum length of the recording is 5 minutes.</span></span> <span data-ttu-id="00418-109">Запись не сохраняется пермаментли платформой Cloud Communications и удаляется вскоре после завершения вызова.</span><span class="sxs-lookup"><span data-stu-id="00418-109">The recording is not saved permamently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="00418-110">Bot должен быстро скачать запись (используя значение **рекординглокатион** , указанное в завершенном уведомлении) после завершения операции записи.</span><span class="sxs-lookup"><span data-stu-id="00418-110">The bot must download the recording promptly (using the **recordingLocation** value given in the completed notification) after the recording operation finishes.</span></span>


## <a name="permissions"></a><span data-ttu-id="00418-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00418-111">Permissions</span></span>
<span data-ttu-id="00418-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00418-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00418-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00418-114">Permission type</span></span> | <span data-ttu-id="00418-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00418-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="00418-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00418-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="00418-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="00418-117">Not Supported</span></span>        |
| <span data-ttu-id="00418-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00418-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00418-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="00418-119">Not Supported</span></span>        |
| <span data-ttu-id="00418-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00418-120">Application</span></span>     | <span data-ttu-id="00418-121">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="00418-121">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="00418-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00418-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="00418-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00418-123">Request headers</span></span>
| <span data-ttu-id="00418-124">Имя</span><span class="sxs-lookup"><span data-stu-id="00418-124">Name</span></span>          | <span data-ttu-id="00418-125">Описание</span><span class="sxs-lookup"><span data-stu-id="00418-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="00418-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00418-126">Authorization</span></span> | <span data-ttu-id="00418-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00418-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00418-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00418-129">Request body</span></span>
<span data-ttu-id="00418-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="00418-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="00418-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="00418-131">Parameter</span></span>      | <span data-ttu-id="00418-132">Тип</span><span class="sxs-lookup"><span data-stu-id="00418-132">Type</span></span>    |<span data-ttu-id="00418-133">Описание</span><span class="sxs-lookup"><span data-stu-id="00418-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00418-134">выдан</span><span class="sxs-lookup"><span data-stu-id="00418-134">prompts</span></span>|<span data-ttu-id="00418-135">Коллекция [медиапромпт](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="00418-135">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="00418-136">Коллекция приглашений для воспроизведения (при наличии) до начала записи.</span><span class="sxs-lookup"><span data-stu-id="00418-136">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="00418-137">Пользователи могут указать действие "Плайпромпт" отдельно или указать его как часть "запись", в основном все записи прецеедед по приглашению.</span><span class="sxs-lookup"><span data-stu-id="00418-137">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt.</span></span> <span data-ttu-id="00418-138">Текущая поддержка предназначена только для одного приглашения в коллекции.</span><span class="sxs-lookup"><span data-stu-id="00418-138">Current support is only for a single prompt as part of the collection.</span></span> |
|<span data-ttu-id="00418-139">Баржеиналловед</span><span class="sxs-lookup"><span data-stu-id="00418-139">bargeInAllowed</span></span>|<span data-ttu-id="00418-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="00418-140">Boolean</span></span>| <span data-ttu-id="00418-141">Если задано значение true, этот запрос будет барже в другие существующие запросы записи и плайпромпт, находящиеся в очереди.</span><span class="sxs-lookup"><span data-stu-id="00418-141">If true, this record request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="00418-142">Значение по умолчанию = false.</span><span class="sxs-lookup"><span data-stu-id="00418-142">Default = false.</span></span> |
|<span data-ttu-id="00418-143">Инитиалсиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="00418-143">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="00418-144">Int32</span><span class="sxs-lookup"><span data-stu-id="00418-144">Int32</span></span>| <span data-ttu-id="00418-145">Максимальное время ожидания (тишины пользователя), разрешенное с момента запуска операции записи до истечения времени ожидания и неудачи операции.</span><span class="sxs-lookup"><span data-stu-id="00418-145">Maximum initial silence (user silence) allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="00418-146">При воспроизведении приглашения этот таймер запускается после завершения приглашения.</span><span class="sxs-lookup"><span data-stu-id="00418-146">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="00418-147">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 300 секунд</span><span class="sxs-lookup"><span data-stu-id="00418-147">Default = 5 seconds, Min = 1 second, Max = 300 seconds</span></span> |
|<span data-ttu-id="00418-148">Макссиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="00418-148">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="00418-149">Int32</span><span class="sxs-lookup"><span data-stu-id="00418-149">Int32</span></span>| <span data-ttu-id="00418-150">Максимально допустимое время тишины (пауза) после начала диктовки пользователя.</span><span class="sxs-lookup"><span data-stu-id="00418-150">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="00418-151">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 300 секунд.</span><span class="sxs-lookup"><span data-stu-id="00418-151">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="00418-152">Максрекорддуратионинсекондс</span><span class="sxs-lookup"><span data-stu-id="00418-152">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="00418-153">Int32</span><span class="sxs-lookup"><span data-stu-id="00418-153">Int32</span></span>| <span data-ttu-id="00418-154">Максимальная длительность операции записи перед остановкой записи.</span><span class="sxs-lookup"><span data-stu-id="00418-154">Max duration for a record operation before stopping recording.</span></span> <span data-ttu-id="00418-155">Значение по умолчанию = 5 секунд, минимум = 1 секунда, максимум = 300 секунд.</span><span class="sxs-lookup"><span data-stu-id="00418-155">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="00418-156">Плайбип</span><span class="sxs-lookup"><span data-stu-id="00418-156">playBeep</span></span>|<span data-ttu-id="00418-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="00418-157">Boolean</span></span>| <span data-ttu-id="00418-158">Если этот параметр имеет значение true, воспроизводит звуковой сигнал, указывающий пользователю, что он может начать запись сообщения.</span><span class="sxs-lookup"><span data-stu-id="00418-158">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="00418-159">Значение по умолчанию = true.</span><span class="sxs-lookup"><span data-stu-id="00418-159">Default = true.</span></span>|
|<span data-ttu-id="00418-160">Стоптонес</span><span class="sxs-lookup"><span data-stu-id="00418-160">stopTones</span></span>|<span data-ttu-id="00418-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="00418-161">String collection</span></span>|<span data-ttu-id="00418-162">Остановка заданных тонов в конец записи.</span><span class="sxs-lookup"><span data-stu-id="00418-162">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="00418-163">Контекст</span><span class="sxs-lookup"><span data-stu-id="00418-163">clientContext</span></span>|<span data-ttu-id="00418-164">String</span><span class="sxs-lookup"><span data-stu-id="00418-164">String</span></span>|<span data-ttu-id="00418-165">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="00418-165">Unique Client Context string.</span></span> <span data-ttu-id="00418-166">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="00418-166">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="00418-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="00418-167">Response</span></span>
<span data-ttu-id="00418-168">Этот метод возвращает код `200 OK` отклика и заголовок Location с URI для [рекордоператион](../resources/recordoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="00418-168">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="00418-169">Пример</span><span class="sxs-lookup"><span data-stu-id="00418-169">Example</span></span>
<span data-ttu-id="00418-170">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="00418-170">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="00418-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="00418-171">Request</span></span>
<span data-ttu-id="00418-172">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00418-172">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="00418-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="00418-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/record
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00418-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="00418-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="00418-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="00418-175">Response</span></span>
<span data-ttu-id="00418-176">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00418-176">The following example shows the response.</span></span>

> <span data-ttu-id="00418-p112">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00418-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "completionReason": null,
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="00418-179">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="00418-179">Notification - operation completed</span></span>

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
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
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

##### <a name="get-recording-file---request"></a><span data-ttu-id="00418-180">Получение файла для записи</span><span class="sxs-lookup"><span data-stu-id="00418-180">Get recording file - Request</span></span>
<span data-ttu-id="00418-181">В приведенном ниже примере показан запрос на получение содержимого записи.</span><span class="sxs-lookup"><span data-stu-id="00418-181">The following example shows the request to get the content of the recording.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="get-recording-file---response"></a><span data-ttu-id="00418-182">Получение файла записи — ответ</span><span class="sxs-lookup"><span data-stu-id="00418-182">Get recording file - Response</span></span>
<span data-ttu-id="00418-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00418-183">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
  "truncated": true
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
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
