---
title: 'вызов: playPrompt'
description: Воспроизведение запрос в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bd2ba6430e6c49039d32a54413e03bd27be574f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951259"
---
# <a name="call-playprompt"></a><span data-ttu-id="6242c-103">вызов: playPrompt</span><span class="sxs-lookup"><span data-stu-id="6242c-103">call: playPrompt</span></span>

> <span data-ttu-id="6242c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6242c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6242c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6242c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6242c-106">Воспроизведение запрос в вызове.</span><span class="sxs-lookup"><span data-stu-id="6242c-106">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6242c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6242c-107">Permissions</span></span>
<span data-ttu-id="6242c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6242c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6242c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6242c-110">Permission type</span></span>                        | <span data-ttu-id="6242c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6242c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6242c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6242c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6242c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6242c-113">Not Supported.</span></span>                               |
| <span data-ttu-id="6242c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6242c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6242c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6242c-115">Not Supported.</span></span>                               |
| <span data-ttu-id="6242c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6242c-116">Application</span></span>                            | <span data-ttu-id="6242c-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6242c-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="6242c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6242c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="6242c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6242c-119">Request headers</span></span>
| <span data-ttu-id="6242c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6242c-120">Name</span></span>          | <span data-ttu-id="6242c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6242c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6242c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6242c-122">Authorization</span></span> | <span data-ttu-id="6242c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6242c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6242c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6242c-125">Request body</span></span>
<span data-ttu-id="6242c-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6242c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6242c-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="6242c-127">Parameter</span></span>      | <span data-ttu-id="6242c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="6242c-128">Type</span></span>    |<span data-ttu-id="6242c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6242c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6242c-130">запросы</span><span class="sxs-lookup"><span data-stu-id="6242c-130">prompts</span></span>|<span data-ttu-id="6242c-131">[запрос](../resources/prompt.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="6242c-131">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="6242c-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="6242c-132">clientContext</span></span>|<span data-ttu-id="6242c-133">String</span><span class="sxs-lookup"><span data-stu-id="6242c-133">String</span></span>|<span data-ttu-id="6242c-134">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="6242c-134">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="6242c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6242c-135">Response</span></span>
<span data-ttu-id="6242c-136">Успешно завершена, этот метод возвращает `200 OK` объект [playPromptOperation](../resources/playPromptOperation.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6242c-136">If successful, this method returns `200 OK` response code and [playPromptOperation](../resources/playPromptOperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6242c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="6242c-137">Example</span></span>
<span data-ttu-id="6242c-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6242c-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6242c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6242c-139">Request</span></span>
<span data-ttu-id="6242c-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6242c-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/playPrompt
Content-Type: application/json
Content-Length: 166

{
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
  ]
}
```

##### <a name="response"></a><span data-ttu-id="6242c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6242c-141">Response</span></span>

> <span data-ttu-id="6242c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6242c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="6242c-144">Уведомления - операция завершена</span><span class="sxs-lookup"><span data-stu-id="6242c-144">Notification - operation completed</span></span>

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
        "@odata.type": "#microsoft.graph.playPromptOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
