---
title: 'вызов: cancelMediaProcessing'
description: Отменяет обработку мультимедиа для выполнения операций playPrompt или recordResponse.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fe6ecbedcb0d66e5261f08eb3a4aee48db25a493
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047667"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="2a11c-103">вызов: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="2a11c-103">call: cancelMediaProcessing</span></span>

<span data-ttu-id="2a11c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a11c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a11c-105">Отменяет обработку для любых операций мультимедиа в ходе выполнения.</span><span class="sxs-lookup"><span data-stu-id="2a11c-105">Cancels processing for any in-progress media operations.</span></span>

<span data-ttu-id="2a11c-106">Операции мультимедиа относятся к операциям IVR [playPrompt](./call-playprompt.md) и [recordResponse,](./call-record.md)которые по умолчанию находятся в очереди для обработки в порядке.</span><span class="sxs-lookup"><span data-stu-id="2a11c-106">Media operations refer to the IVR operations [playPrompt](./call-playprompt.md) and [recordResponse](./call-record.md), which are by default queued to process in order.</span></span> <span data-ttu-id="2a11c-107">Метод **cancelMediaProcessing** отменяет все операции, которые находятся в процессе, а также операции, которые находятся в очереди.</span><span class="sxs-lookup"><span data-stu-id="2a11c-107">The **cancelMediaProcessing** method cancels any operation that is in-process as well as operations that are queued.</span></span> <span data-ttu-id="2a11c-108">Например, этот API можно использовать для очистки очереди операции IVR для новой операции мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="2a11c-108">For example, this API can be used to clean up the IVR operation queue for a new media operation.</span></span> <span data-ttu-id="2a11c-109">Однако операция **ubscribeToTone** не отменяется, так как она работает независимо от очереди операции.</span><span class="sxs-lookup"><span data-stu-id="2a11c-109">However, it will not cancel a **ubscribeToTone** operation because it operates independent of any operation queue.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a11c-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a11c-110">Permissions</span></span>
<span data-ttu-id="2a11c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a11c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a11c-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a11c-113">Permission type</span></span>                        | <span data-ttu-id="2a11c-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a11c-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a11c-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a11c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a11c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a11c-116">Not Supported.</span></span>                              |
| <span data-ttu-id="2a11c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a11c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a11c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a11c-118">Not Supported.</span></span>                              |
| <span data-ttu-id="2a11c-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a11c-119">Application</span></span>                            | <span data-ttu-id="2a11c-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2a11c-120">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="2a11c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a11c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="2a11c-122">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="2a11c-122">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="2a11c-123">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="2a11c-123">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a11c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a11c-124">Request headers</span></span>
| <span data-ttu-id="2a11c-125">Имя</span><span class="sxs-lookup"><span data-stu-id="2a11c-125">Name</span></span>          | <span data-ttu-id="2a11c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="2a11c-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2a11c-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a11c-127">Authorization</span></span> | <span data-ttu-id="2a11c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a11c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a11c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a11c-130">Content-type</span></span> | <span data-ttu-id="2a11c-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a11c-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a11c-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a11c-133">Request body</span></span>
<span data-ttu-id="2a11c-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2a11c-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2a11c-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="2a11c-135">Parameter</span></span>      | <span data-ttu-id="2a11c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="2a11c-136">Type</span></span>    | <span data-ttu-id="2a11c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="2a11c-137">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="2a11c-138">clientContext</span><span class="sxs-lookup"><span data-stu-id="2a11c-138">clientContext</span></span>  | <span data-ttu-id="2a11c-139">String</span><span class="sxs-lookup"><span data-stu-id="2a11c-139">String</span></span>  | <span data-ttu-id="2a11c-140">Клиентский контекст.</span><span class="sxs-lookup"><span data-stu-id="2a11c-140">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="2a11c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a11c-141">Response</span></span>
<span data-ttu-id="2a11c-142">В случае успешной работы этот метод возвращает код отклика HTTP и заглавную головку расположения с URI в `200 OK` [commsOperation,](../resources/commsoperation.md) созданный для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="2a11c-142">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="2a11c-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2a11c-143">Example</span></span>
<span data-ttu-id="2a11c-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="2a11c-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2a11c-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a11c-145">Request</span></span>
<span data-ttu-id="2a11c-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a11c-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a11c-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a11c-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[<span data-ttu-id="2a11c-148">C#</span><span class="sxs-lookup"><span data-stu-id="2a11c-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a11c-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a11c-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a11c-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a11c-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a11c-151">Java</span><span class="sxs-lookup"><span data-stu-id="2a11c-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-cancelmediaprocessing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2a11c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a11c-152">Response</span></span>

> <span data-ttu-id="2a11c-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2a11c-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.cancelMediaProcessingOperation",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5"
}
```

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="2a11c-154">Уведомление — отмена операции для recordResponse</span><span class="sxs-lookup"><span data-stu-id="2a11c-154">Notification - Operation canceled for recordResponse</span></span>

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
        "status": "failed",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 400,
          "subcode": 8508,
          "message": "Action failed, the operation was cancelled."
        },
        "recordingLocation": "",
        "recordingAccessToken": "",
        "completionReason": "operationCanceled"
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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


