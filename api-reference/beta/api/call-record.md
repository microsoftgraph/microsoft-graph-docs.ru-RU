---
title: 'Call: Record'
description: Запись вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fad06769f81b9840b89a43cf3e759c86454edef0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438631"
---
# <a name="call-record"></a><span data-ttu-id="11793-103">Call: Record</span><span class="sxs-lookup"><span data-stu-id="11793-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11793-104">Запись вызова.</span><span class="sxs-lookup"><span data-stu-id="11793-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="11793-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11793-105">Permissions</span></span>
<span data-ttu-id="11793-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11793-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11793-108">Permission type</span></span> | <span data-ttu-id="11793-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11793-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="11793-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11793-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="11793-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="11793-111">Not Supported</span></span>        |
| <span data-ttu-id="11793-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11793-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11793-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="11793-113">Not Supported</span></span>        |
| <span data-ttu-id="11793-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11793-114">Application</span></span>     | <span data-ttu-id="11793-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="11793-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="11793-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11793-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="11793-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11793-117">Request headers</span></span>
| <span data-ttu-id="11793-118">Имя</span><span class="sxs-lookup"><span data-stu-id="11793-118">Name</span></span>          | <span data-ttu-id="11793-119">Описание</span><span class="sxs-lookup"><span data-stu-id="11793-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="11793-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11793-120">Authorization</span></span> | <span data-ttu-id="11793-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11793-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11793-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="11793-123">Request body</span></span>
<span data-ttu-id="11793-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="11793-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11793-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="11793-125">Parameter</span></span>      | <span data-ttu-id="11793-126">Тип</span><span class="sxs-lookup"><span data-stu-id="11793-126">Type</span></span>    |<span data-ttu-id="11793-127">Описание</span><span class="sxs-lookup"><span data-stu-id="11793-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11793-128">выдан</span><span class="sxs-lookup"><span data-stu-id="11793-128">prompts</span></span>|<span data-ttu-id="11793-129">Коллекция [медиапромпт](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="11793-129">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="11793-130">Коллекция приглашений для воспроизведения (при наличии) до начала записи.</span><span class="sxs-lookup"><span data-stu-id="11793-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="11793-131">Пользователи могут указать действие "Плайпромпт" отдельно или указать его как часть "запись", в основном все записи прецеедед по запросу.</span><span class="sxs-lookup"><span data-stu-id="11793-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="11793-132">Баржеиналловед</span><span class="sxs-lookup"><span data-stu-id="11793-132">bargeInAllowed</span></span>|<span data-ttu-id="11793-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="11793-133">Boolean</span></span>| <span data-ttu-id="11793-134">Разрешить пользователям вводить варианты до завершения приглашения.</span><span class="sxs-lookup"><span data-stu-id="11793-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="11793-135">Инитиалсиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="11793-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="11793-136">Int32</span><span class="sxs-lookup"><span data-stu-id="11793-136">Int32</span></span>| <span data-ttu-id="11793-137">Максимально допустимое время простоя при запуске операции записи до истечения времени ожидания и отказа операции.</span><span class="sxs-lookup"><span data-stu-id="11793-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="11793-138">При воспроизведении приглашения этот таймер запускается после завершения приглашения.</span><span class="sxs-lookup"><span data-stu-id="11793-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="11793-139">Макссиленцетимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="11793-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="11793-140">Int32</span><span class="sxs-lookup"><span data-stu-id="11793-140">Int32</span></span>| <span data-ttu-id="11793-141">Максимальное время ожидания тишины в секундах.</span><span class="sxs-lookup"><span data-stu-id="11793-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="11793-142">Максрекорддуратионинсекондс</span><span class="sxs-lookup"><span data-stu-id="11793-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="11793-143">Int32</span><span class="sxs-lookup"><span data-stu-id="11793-143">Int32</span></span>| <span data-ttu-id="11793-144">Максимальная длительность записи в секундах.</span><span class="sxs-lookup"><span data-stu-id="11793-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="11793-145">Плайбип</span><span class="sxs-lookup"><span data-stu-id="11793-145">playBeep</span></span>|<span data-ttu-id="11793-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="11793-146">Boolean</span></span>| <span data-ttu-id="11793-147">Воспроизводит звуковой сигнал после воспроизведения приглашения.</span><span class="sxs-lookup"><span data-stu-id="11793-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="11793-148">Стреамвхилерекординг</span><span class="sxs-lookup"><span data-stu-id="11793-148">streamWhileRecording</span></span>|<span data-ttu-id="11793-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="11793-149">Boolean</span></span>|<span data-ttu-id="11793-150">Если задано значение true, расположение ресурса будет указано сразу после начала записи.</span><span class="sxs-lookup"><span data-stu-id="11793-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="11793-151">Стоптонес</span><span class="sxs-lookup"><span data-stu-id="11793-151">stopTones</span></span>|<span data-ttu-id="11793-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="11793-152">String collection</span></span>|<span data-ttu-id="11793-153">Остановка заданных тонов в конец записи.</span><span class="sxs-lookup"><span data-stu-id="11793-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="11793-154">Контекст</span><span class="sxs-lookup"><span data-stu-id="11793-154">clientContext</span></span>|<span data-ttu-id="11793-155">String</span><span class="sxs-lookup"><span data-stu-id="11793-155">String</span></span>|<span data-ttu-id="11793-156">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="11793-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="11793-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="11793-157">Response</span></span>
<span data-ttu-id="11793-158">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="11793-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="11793-159">Пример</span><span class="sxs-lookup"><span data-stu-id="11793-159">Example</span></span>
<span data-ttu-id="11793-160">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="11793-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="11793-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="11793-161">Request</span></span>
<span data-ttu-id="11793-162">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11793-162">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="11793-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="11793-163">HTTP</span></span>](#tab/http)
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
      },
      "loop": 5
    }
  ],
  "maxRecordDurationInSeconds": 1800,
  "initialSilenceTimeoutInSeconds": 10,
  "maxSilenceTimeoutInSeconds": 2,
  "recordingFormat": "wav",
  "playBeep": true,
  "streamWhileRecording": true,
  "stopTones": [ "#", "11", "*" ]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11793-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="11793-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="11793-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="11793-165">Response</span></span>

> <span data-ttu-id="11793-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11793-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="11793-168">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="11793-168">Notification - operation completed</span></span>

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
        "recordResourceLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordResourceAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
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
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
