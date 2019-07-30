---
title: 'Call: Плайпромпт'
description: Проигрывать запрос в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cc65ed5b9ced14cd259bf678ee1152089d654e2c
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931100"
---
# <a name="call-playprompt"></a><span data-ttu-id="62d36-103">Call: Плайпромпт</span><span class="sxs-lookup"><span data-stu-id="62d36-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62d36-104">Проигрывать запрос в вызове.</span><span class="sxs-lookup"><span data-stu-id="62d36-104">Play a prompt in the call.</span></span>

<span data-ttu-id="62d36-105">Дополнительные сведения об обработке операций можно найти в статье [коммсоператион](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="62d36-105">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="62d36-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62d36-106">Permissions</span></span>
<span data-ttu-id="62d36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62d36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62d36-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62d36-109">Permission type</span></span>                        | <span data-ttu-id="62d36-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62d36-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62d36-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62d36-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62d36-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62d36-112">Not Supported.</span></span>                               |
| <span data-ttu-id="62d36-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62d36-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62d36-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62d36-114">Not Supported.</span></span>                               |
| <span data-ttu-id="62d36-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="62d36-115">Application</span></span>                            | <span data-ttu-id="62d36-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="62d36-116">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="62d36-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62d36-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="62d36-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62d36-118">Request headers</span></span>
| <span data-ttu-id="62d36-119">Имя</span><span class="sxs-lookup"><span data-stu-id="62d36-119">Name</span></span>          | <span data-ttu-id="62d36-120">Описание</span><span class="sxs-lookup"><span data-stu-id="62d36-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="62d36-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62d36-121">Authorization</span></span> | <span data-ttu-id="62d36-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62d36-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62d36-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62d36-124">Request body</span></span>
<span data-ttu-id="62d36-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="62d36-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="62d36-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="62d36-126">Parameter</span></span>      | <span data-ttu-id="62d36-127">Тип</span><span class="sxs-lookup"><span data-stu-id="62d36-127">Type</span></span>    |<span data-ttu-id="62d36-128">Описание</span><span class="sxs-lookup"><span data-stu-id="62d36-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62d36-129">выдан</span><span class="sxs-lookup"><span data-stu-id="62d36-129">prompts</span></span>|<span data-ttu-id="62d36-130">Коллекция [Prompt](../resources/prompt.md)</span><span class="sxs-lookup"><span data-stu-id="62d36-130">[prompt](../resources/prompt.md) collection</span></span>| <span data-ttu-id="62d36-131">В настоящее время поддерживается только один запрос и тип [медиапромпт](../resources/mediaprompt.md) .</span><span class="sxs-lookup"><span data-stu-id="62d36-131">Currently only a single prompt and of type [MediaPrompt](../resources/mediaprompt.md) is supported.</span></span>|
|<span data-ttu-id="62d36-132">CNAME</span><span class="sxs-lookup"><span data-stu-id="62d36-132">loop</span></span>|<span data-ttu-id="62d36-133">bool</span><span class="sxs-lookup"><span data-stu-id="62d36-133">bool</span></span>| <span data-ttu-id="62d36-134">Значение цикла.</span><span class="sxs-lookup"><span data-stu-id="62d36-134">The loop value.</span></span> <span data-ttu-id="62d36-135">значение true указывает, что цикл должен быть бесконечным.</span><span class="sxs-lookup"><span data-stu-id="62d36-135">true indicates to loop infinitely.</span></span> <span data-ttu-id="62d36-136">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="62d36-136">The default value is false.</span></span> |
|<span data-ttu-id="62d36-137">Контекст</span><span class="sxs-lookup"><span data-stu-id="62d36-137">clientContext</span></span>|<span data-ttu-id="62d36-138">String</span><span class="sxs-lookup"><span data-stu-id="62d36-138">String</span></span>|<span data-ttu-id="62d36-139">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="62d36-139">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="62d36-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="62d36-140">Response</span></span>
<span data-ttu-id="62d36-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [плайпромптоператион](../resources/playpromptoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62d36-141">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62d36-142">Пример</span><span class="sxs-lookup"><span data-stu-id="62d36-142">Example</span></span>
<span data-ttu-id="62d36-143">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="62d36-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="62d36-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="62d36-144">Request</span></span>
<span data-ttu-id="62d36-145">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62d36-145">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="62d36-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="62d36-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "@odata.type": "#microsoft.graph.mediaInfo",
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
    },
  ],
  "loop": false
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62d36-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="62d36-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="62d36-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="62d36-148">Response</span></span>

> <span data-ttu-id="62d36-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62d36-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="62d36-151">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="62d36-151">Notification - operation completed</span></span>

 ><span data-ttu-id="62d36-152">**Примечание:** При возникновении бесконечного цикла это уведомление не отправляется.</span><span class="sxs-lookup"><span data-stu-id="62d36-152">**Note:** If infinite looping occurs, this notification is not sent.</span></span>
 
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
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
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
<!--
{
  "type": "#page.annotation",
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
