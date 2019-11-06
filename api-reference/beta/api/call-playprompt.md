---
title: 'Call: Плайпромпт'
description: Проигрывать запрос в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 465cd7a0695d7c8dee510b68a75c8b08b99cdc31
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005985"
---
# <a name="call-playprompt"></a><span data-ttu-id="04776-103">Call: Плайпромпт</span><span class="sxs-lookup"><span data-stu-id="04776-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04776-104">Проигрывать запрос в вызове.</span><span class="sxs-lookup"><span data-stu-id="04776-104">Play a prompt in the call.</span></span>

<span data-ttu-id="04776-105">Дополнительные сведения об обработке операций можно найти в статье [коммсоператион](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="04776-105">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="04776-106">Действие **плайпромпт** поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="04776-106">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="04776-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04776-107">Permissions</span></span>
<span data-ttu-id="04776-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04776-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04776-110">Permission type</span></span>                        | <span data-ttu-id="04776-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04776-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="04776-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04776-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="04776-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04776-113">Not Supported.</span></span>                               |
| <span data-ttu-id="04776-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04776-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04776-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04776-115">Not Supported.</span></span>                               |
| <span data-ttu-id="04776-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04776-116">Application</span></span>                            | <span data-ttu-id="04776-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="04776-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="04776-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04776-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /communications/calls/{id}/playPrompt
```
> <span data-ttu-id="04776-119">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="04776-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="04776-120">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="04776-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04776-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04776-121">Request headers</span></span>
| <span data-ttu-id="04776-122">Имя</span><span class="sxs-lookup"><span data-stu-id="04776-122">Name</span></span>          | <span data-ttu-id="04776-123">Описание</span><span class="sxs-lookup"><span data-stu-id="04776-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="04776-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04776-124">Authorization</span></span> | <span data-ttu-id="04776-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04776-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04776-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04776-127">Request body</span></span>
<span data-ttu-id="04776-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="04776-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04776-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="04776-129">Parameter</span></span>      | <span data-ttu-id="04776-130">Тип</span><span class="sxs-lookup"><span data-stu-id="04776-130">Type</span></span>    |<span data-ttu-id="04776-131">Описание</span><span class="sxs-lookup"><span data-stu-id="04776-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04776-132">выдан</span><span class="sxs-lookup"><span data-stu-id="04776-132">prompts</span></span>|<span data-ttu-id="04776-133">Коллекция Медиапромпт</span><span class="sxs-lookup"><span data-stu-id="04776-133">MediaPrompt collection</span></span>| <span data-ttu-id="04776-134">В настоящее время поддерживается только один запрос и тип [медиапромпт](../resources/mediaprompt.md) .</span><span class="sxs-lookup"><span data-stu-id="04776-134">Currently only a single prompt and of type [MediaPrompt](../resources/mediaprompt.md) is supported.</span></span>|
|<span data-ttu-id="04776-135">CNAME</span><span class="sxs-lookup"><span data-stu-id="04776-135">loop</span></span>|<span data-ttu-id="04776-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="04776-136">Boolean</span></span>| <span data-ttu-id="04776-137">Значение цикла.</span><span class="sxs-lookup"><span data-stu-id="04776-137">The loop value.</span></span> <span data-ttu-id="04776-138">Значение true указывает, что цикл должен быть бесконечным.</span><span class="sxs-lookup"><span data-stu-id="04776-138">True indicates to loop infinitely.</span></span> <span data-ttu-id="04776-139">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="04776-139">The default value is false.</span></span> |
|<span data-ttu-id="04776-140">Контекст</span><span class="sxs-lookup"><span data-stu-id="04776-140">clientContext</span></span>|<span data-ttu-id="04776-141">String</span><span class="sxs-lookup"><span data-stu-id="04776-141">String</span></span>|<span data-ttu-id="04776-142">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="04776-142">Unique client context string.</span></span> <span data-ttu-id="04776-143">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="04776-143">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="04776-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="04776-144">Response</span></span>
<span data-ttu-id="04776-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [плайпромптоператион](../resources/playpromptoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04776-145">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04776-146">Пример</span><span class="sxs-lookup"><span data-stu-id="04776-146">Example</span></span>
<span data-ttu-id="04776-147">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="04776-147">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="04776-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="04776-148">Request</span></span>
<span data-ttu-id="04776-149">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04776-149">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="04776-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="04776-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04776-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04776-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04776-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="04776-152">Response</span></span>
<span data-ttu-id="04776-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04776-153">The following is an example of the response.</span></span>

> <span data-ttu-id="04776-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04776-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="04776-156">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="04776-156">Notification - operation completed</span></span>

 ><span data-ttu-id="04776-157">**Примечание:** При возникновении бесконечного цикла это уведомление не отправляется.</span><span class="sxs-lookup"><span data-stu-id="04776-157">**Note:** If infinite looping occurs, this notification is not sent.</span></span>
 
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
        "@odata.type": "#microsoft.graph.playPromptOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
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
