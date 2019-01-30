---
title: 'Вызовите: записи'
description: Запись вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4dc409a502b18da9c0e897054a7c1d6386fa096f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641906"
---
# <a name="call-record"></a><span data-ttu-id="11c4b-103">Вызовите: записи</span><span class="sxs-lookup"><span data-stu-id="11c4b-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11c4b-104">Запись вызова.</span><span class="sxs-lookup"><span data-stu-id="11c4b-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="11c4b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11c4b-105">Permissions</span></span>
<span data-ttu-id="11c4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11c4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11c4b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11c4b-108">Permission type</span></span> | <span data-ttu-id="11c4b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11c4b-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="11c4b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11c4b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="11c4b-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="11c4b-111">Not Supported</span></span>        |
| <span data-ttu-id="11c4b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11c4b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11c4b-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="11c4b-113">Not Supported</span></span>        |
| <span data-ttu-id="11c4b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11c4b-114">Application</span></span>     | <span data-ttu-id="11c4b-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="11c4b-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="11c4b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11c4b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="11c4b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11c4b-117">Request headers</span></span>
| <span data-ttu-id="11c4b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="11c4b-118">Name</span></span>          | <span data-ttu-id="11c4b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="11c4b-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="11c4b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11c4b-120">Authorization</span></span> | <span data-ttu-id="11c4b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11c4b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11c4b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="11c4b-123">Request body</span></span>
<span data-ttu-id="11c4b-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="11c4b-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11c4b-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="11c4b-125">Parameter</span></span>      | <span data-ttu-id="11c4b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="11c4b-126">Type</span></span>    |<span data-ttu-id="11c4b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="11c4b-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11c4b-128">запросы</span><span class="sxs-lookup"><span data-stu-id="11c4b-128">prompts</span></span>|<span data-ttu-id="11c4b-129">[mediaprompt](../resources/mediaprompt.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="11c4b-129">[mediaprompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="11c4b-130">Коллекция запросы на воспроизведение (если они имеются) перед записи запускается.</span><span class="sxs-lookup"><span data-stu-id="11c4b-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="11c4b-131">Клиенты могут вести указывает действие «playPrompt» отдельно или как часть «запись» - большей части все записи, перед с помощью строки</span><span class="sxs-lookup"><span data-stu-id="11c4b-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="11c4b-132">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="11c4b-132">bargeInAllowed</span></span>|<span data-ttu-id="11c4b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="11c4b-133">Boolean</span></span>| <span data-ttu-id="11c4b-134">Разрешить пользователям вариант до завершения строки.</span><span class="sxs-lookup"><span data-stu-id="11c4b-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="11c4b-135">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="11c4b-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="11c4b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="11c4b-136">Int32</span></span>| <span data-ttu-id="11c4b-137">Допускается с момента времени ожидания и происходит сбой операции начинаем операцию записи, прежде чем мы максимальное начальной бездействия.</span><span class="sxs-lookup"><span data-stu-id="11c4b-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="11c4b-138">Если воспроизводится запрос этот таймер запускается после завершения строки.</span><span class="sxs-lookup"><span data-stu-id="11c4b-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="11c4b-139">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="11c4b-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="11c4b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="11c4b-140">Int32</span></span>| <span data-ttu-id="11c4b-141">Бездействия максимальное время ожидания в секундах.</span><span class="sxs-lookup"><span data-stu-id="11c4b-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="11c4b-142">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="11c4b-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="11c4b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="11c4b-143">Int32</span></span>| <span data-ttu-id="11c4b-144">Запись Максимальная длительность в секундах.</span><span class="sxs-lookup"><span data-stu-id="11c4b-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="11c4b-145">playBeep</span><span class="sxs-lookup"><span data-stu-id="11c4b-145">playBeep</span></span>|<span data-ttu-id="11c4b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="11c4b-146">Boolean</span></span>| <span data-ttu-id="11c4b-147">Воспроизводит звуковой сигнал после воспроизведения в строке.</span><span class="sxs-lookup"><span data-stu-id="11c4b-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="11c4b-148">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="11c4b-148">streamWhileRecording</span></span>|<span data-ttu-id="11c4b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="11c4b-149">Boolean</span></span>|<span data-ttu-id="11c4b-150">Если значение равно true, расположение ресурсов будет предоставляются как только начнется регистрация.</span><span class="sxs-lookup"><span data-stu-id="11c4b-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="11c4b-151">stopTones</span><span class="sxs-lookup"><span data-stu-id="11c4b-151">stopTones</span></span>|<span data-ttu-id="11c4b-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="11c4b-152">String collection</span></span>|<span data-ttu-id="11c4b-153">Остановите мелодии, для которого требуется завершить запись.</span><span class="sxs-lookup"><span data-stu-id="11c4b-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="11c4b-154">clientContext</span><span class="sxs-lookup"><span data-stu-id="11c4b-154">clientContext</span></span>|<span data-ttu-id="11c4b-155">String</span><span class="sxs-lookup"><span data-stu-id="11c4b-155">String</span></span>|<span data-ttu-id="11c4b-156">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="11c4b-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="11c4b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="11c4b-157">Response</span></span>
<span data-ttu-id="11c4b-158">Возвращает `202 Accepted` код ответа и расположения заголовком с uri для [commsOperation](../resources/commsoperation.md) , созданные для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="11c4b-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="11c4b-159">Пример</span><span class="sxs-lookup"><span data-stu-id="11c4b-159">Example</span></span>
<span data-ttu-id="11c4b-160">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="11c4b-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="11c4b-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="11c4b-161">Request</span></span>
<span data-ttu-id="11c4b-162">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11c4b-162">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="11c4b-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="11c4b-163">Response</span></span>

> <span data-ttu-id="11c4b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11c4b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="11c4b-166">Уведомления - операция завершена</span><span class="sxs-lookup"><span data-stu-id="11c4b-166">Notification - operation completed</span></span>

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
    "Error: /api-reference/beta/api/call-record.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
