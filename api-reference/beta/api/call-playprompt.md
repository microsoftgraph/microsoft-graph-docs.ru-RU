---
title: 'Call: Плайпромпт'
description: Проигрывать запрос в вызове.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b1e24b0e1d50a3015e6b6ade9de8ccf011e4e23a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440789"
---
# <a name="call-playprompt"></a><span data-ttu-id="79f90-103">Call: Плайпромпт</span><span class="sxs-lookup"><span data-stu-id="79f90-103">call: playPrompt</span></span>

<span data-ttu-id="79f90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79f90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79f90-105">Проигрывать запрос в вызове.</span><span class="sxs-lookup"><span data-stu-id="79f90-105">Play a prompt in the call.</span></span>

<span data-ttu-id="79f90-106">Дополнительные сведения об обработке операций можно найти в статье [коммсоператион](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="79f90-106">For more information about how to handle operations, see [commsOperation](../resources/commsoperation.md)</span></span>

> [!Note]
> <span data-ttu-id="79f90-107">Действие **плайпромпт** поддерживается только для [вызовов](../resources/call.md) , инициированных с помощью [сервицехостедмедиаконфиг](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="79f90-107">The **playPrompt** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79f90-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79f90-108">Permissions</span></span>
<span data-ttu-id="79f90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79f90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79f90-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79f90-111">Permission type</span></span>                        | <span data-ttu-id="79f90-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79f90-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79f90-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79f90-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="79f90-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f90-114">Not Supported.</span></span>                               |
| <span data-ttu-id="79f90-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79f90-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79f90-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f90-116">Not Supported.</span></span>                               |
| <span data-ttu-id="79f90-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79f90-117">Application</span></span>                            | <span data-ttu-id="79f90-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="79f90-118">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="79f90-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79f90-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /communications/calls/{id}/playPrompt
```
> <span data-ttu-id="79f90-120">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="79f90-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="79f90-121">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="79f90-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79f90-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79f90-122">Request headers</span></span>
| <span data-ttu-id="79f90-123">Имя</span><span class="sxs-lookup"><span data-stu-id="79f90-123">Name</span></span>          | <span data-ttu-id="79f90-124">Описание</span><span class="sxs-lookup"><span data-stu-id="79f90-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="79f90-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79f90-125">Authorization</span></span> | <span data-ttu-id="79f90-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79f90-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79f90-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79f90-128">Request body</span></span>
<span data-ttu-id="79f90-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="79f90-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79f90-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="79f90-130">Parameter</span></span>      | <span data-ttu-id="79f90-131">Тип</span><span class="sxs-lookup"><span data-stu-id="79f90-131">Type</span></span>    |<span data-ttu-id="79f90-132">Описание</span><span class="sxs-lookup"><span data-stu-id="79f90-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79f90-133">выдан</span><span class="sxs-lookup"><span data-stu-id="79f90-133">prompts</span></span>|<span data-ttu-id="79f90-134">Коллекция [медиапромпт](../resources/mediaprompt.md)</span><span class="sxs-lookup"><span data-stu-id="79f90-134">[MediaPrompt](../resources/mediaprompt.md) collection</span></span>| <span data-ttu-id="79f90-135">Приглашения для воспроизведения.</span><span class="sxs-lookup"><span data-stu-id="79f90-135">The prompts to be played.</span></span> <span data-ttu-id="79f90-136">Максимальный поддерживаемый размер коллекции Медиапромпт составляет 20.</span><span class="sxs-lookup"><span data-stu-id="79f90-136">The maximum supported mediaPrompt collection size is 20.</span></span>|
|<span data-ttu-id="79f90-137">CNAME</span><span class="sxs-lookup"><span data-stu-id="79f90-137">loop</span></span>|<span data-ttu-id="79f90-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="79f90-138">Boolean</span></span>| <span data-ttu-id="79f90-139">Значение цикла.</span><span class="sxs-lookup"><span data-stu-id="79f90-139">The loop value.</span></span> <span data-ttu-id="79f90-140">Значение true указывает, что цикл должен быть бесконечным.</span><span class="sxs-lookup"><span data-stu-id="79f90-140">True indicates to loop infinitely.</span></span> <span data-ttu-id="79f90-141">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="79f90-141">The default value is false.</span></span> |
|<span data-ttu-id="79f90-142">Контекст</span><span class="sxs-lookup"><span data-stu-id="79f90-142">clientContext</span></span>|<span data-ttu-id="79f90-143">String</span><span class="sxs-lookup"><span data-stu-id="79f90-143">String</span></span>|<span data-ttu-id="79f90-144">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="79f90-144">Unique client context string.</span></span> <span data-ttu-id="79f90-145">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="79f90-145">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="79f90-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="79f90-146">Response</span></span>
<span data-ttu-id="79f90-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [плайпромптоператион](../resources/playpromptoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79f90-147">If successful, this method returns a `200 OK` response code and a [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79f90-148">Пример</span><span class="sxs-lookup"><span data-stu-id="79f90-148">Example</span></span>
<span data-ttu-id="79f90-149">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="79f90-149">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="79f90-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="79f90-150">Request</span></span>
<span data-ttu-id="79f90-151">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79f90-151">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79f90-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="79f90-152">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="79f90-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79f90-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-playprompt-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79f90-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="79f90-154">Response</span></span>
<span data-ttu-id="79f90-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79f90-155">The following is an example of the response.</span></span>

> <span data-ttu-id="79f90-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79f90-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="79f90-158">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="79f90-158">Notification - operation completed</span></span>

 ><span data-ttu-id="79f90-159">**Примечание:** При возникновении бесконечного цикла это уведомление не отправляется.</span><span class="sxs-lookup"><span data-stu-id="79f90-159">**Note:** If infinite looping occurs, this notification is not sent.</span></span>
 
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
