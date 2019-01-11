---
title: 'Вызовите: записи'
description: Запишите вызова.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: afb74bb656eb6fcc09fdab71477843748bc5616d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859579"
---
# <a name="call-record"></a><span data-ttu-id="558c7-103">Вызовите: записи</span><span class="sxs-lookup"><span data-stu-id="558c7-103">call: record</span></span>

> <span data-ttu-id="558c7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="558c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="558c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="558c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="558c7-106">Запишите вызова.</span><span class="sxs-lookup"><span data-stu-id="558c7-106">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="558c7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="558c7-107">Permissions</span></span>
<span data-ttu-id="558c7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="558c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="558c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="558c7-110">Permission type</span></span> | <span data-ttu-id="558c7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="558c7-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="558c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="558c7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="558c7-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="558c7-113">Not Supported</span></span>        |
| <span data-ttu-id="558c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="558c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="558c7-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="558c7-115">Not Supported</span></span>        |
| <span data-ttu-id="558c7-116">Application</span><span class="sxs-lookup"><span data-stu-id="558c7-116">Application</span></span>     | <span data-ttu-id="558c7-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="558c7-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="558c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="558c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="558c7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="558c7-119">Request headers</span></span>
| <span data-ttu-id="558c7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="558c7-120">Name</span></span>          | <span data-ttu-id="558c7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="558c7-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="558c7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="558c7-122">Authorization</span></span> | <span data-ttu-id="558c7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="558c7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="558c7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="558c7-125">Request body</span></span>
<span data-ttu-id="558c7-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="558c7-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="558c7-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="558c7-127">Parameter</span></span>      | <span data-ttu-id="558c7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="558c7-128">Type</span></span>    |<span data-ttu-id="558c7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="558c7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="558c7-130">запросы</span><span class="sxs-lookup"><span data-stu-id="558c7-130">prompts</span></span>|<span data-ttu-id="558c7-131">[mediaprompt](../resources/mediaprompt.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="558c7-131">[mediaprompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="558c7-132">Коллекция запросы на воспроизведение (если они имеются) перед записи запускается.</span><span class="sxs-lookup"><span data-stu-id="558c7-132">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="558c7-133">Клиенты могут вести указывает действие «playPrompt» отдельно или как часть «запись» - большей части все записи, перед с помощью строки</span><span class="sxs-lookup"><span data-stu-id="558c7-133">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="558c7-134">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="558c7-134">bargeInAllowed</span></span>|<span data-ttu-id="558c7-135">Логический</span><span class="sxs-lookup"><span data-stu-id="558c7-135">Boolean</span></span>| <span data-ttu-id="558c7-136">Разрешить пользователям вариант до завершения строки.</span><span class="sxs-lookup"><span data-stu-id="558c7-136">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="558c7-137">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="558c7-137">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="558c7-138">Int32</span><span class="sxs-lookup"><span data-stu-id="558c7-138">Int32</span></span>| <span data-ttu-id="558c7-139">Допускается с момента времени ожидания и происходит сбой операции начинаем операцию записи, прежде чем мы максимальное начальной бездействия.</span><span class="sxs-lookup"><span data-stu-id="558c7-139">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="558c7-140">Если воспроизводится запрос этот таймер запускается после завершения строки.</span><span class="sxs-lookup"><span data-stu-id="558c7-140">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="558c7-141">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="558c7-141">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="558c7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="558c7-142">Int32</span></span>| <span data-ttu-id="558c7-143">Бездействия максимальное время ожидания в секундах.</span><span class="sxs-lookup"><span data-stu-id="558c7-143">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="558c7-144">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="558c7-144">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="558c7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="558c7-145">Int32</span></span>| <span data-ttu-id="558c7-146">Запись Максимальная длительность в секундах.</span><span class="sxs-lookup"><span data-stu-id="558c7-146">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="558c7-147">playBeep</span><span class="sxs-lookup"><span data-stu-id="558c7-147">playBeep</span></span>|<span data-ttu-id="558c7-148">Логический</span><span class="sxs-lookup"><span data-stu-id="558c7-148">Boolean</span></span>| <span data-ttu-id="558c7-149">Воспроизводит звуковой сигнал после воспроизведения в строке.</span><span class="sxs-lookup"><span data-stu-id="558c7-149">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="558c7-150">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="558c7-150">streamWhileRecording</span></span>|<span data-ttu-id="558c7-151">Логический</span><span class="sxs-lookup"><span data-stu-id="558c7-151">Boolean</span></span>|<span data-ttu-id="558c7-152">Если значение равно true, расположение ресурсов будет предоставляются как только начнется регистрация.</span><span class="sxs-lookup"><span data-stu-id="558c7-152">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="558c7-153">stopTones</span><span class="sxs-lookup"><span data-stu-id="558c7-153">stopTones</span></span>|<span data-ttu-id="558c7-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="558c7-154">String collection</span></span>|<span data-ttu-id="558c7-155">Остановите мелодии, для которого требуется завершить запись.</span><span class="sxs-lookup"><span data-stu-id="558c7-155">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="558c7-156">clientContext</span><span class="sxs-lookup"><span data-stu-id="558c7-156">clientContext</span></span>|<span data-ttu-id="558c7-157">Строка</span><span class="sxs-lookup"><span data-stu-id="558c7-157">String</span></span>|<span data-ttu-id="558c7-158">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="558c7-158">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="558c7-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="558c7-159">Response</span></span>
<span data-ttu-id="558c7-160">Возвращает `202 Accepted` код ответа и расположения заголовком с uri для [commsOperation](../resources/commsoperation.md) , созданные для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="558c7-160">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="558c7-161">Пример</span><span class="sxs-lookup"><span data-stu-id="558c7-161">Example</span></span>
<span data-ttu-id="558c7-162">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="558c7-162">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="558c7-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="558c7-163">Request</span></span>
<span data-ttu-id="558c7-164">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="558c7-164">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="558c7-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="558c7-165">Response</span></span>

> <span data-ttu-id="558c7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="558c7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="558c7-168">Уведомления - операция завершена</span><span class="sxs-lookup"><span data-stu-id="558c7-168">Notification - operation completed</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
