---
title: 'Call: Канцелмедиапроцессинг'
description: Отменяет обработку мультимедиа для всех выполняющихся операций Плайпромпт или Рекордреспонсе.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 695b7e235e4337c2d7550668bd6be4996efe335f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959830"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="e4f8a-103">Call: Канцелмедиапроцессинг</span><span class="sxs-lookup"><span data-stu-id="e4f8a-103">call: cancelMediaProcessing</span></span>

<span data-ttu-id="e4f8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f8a-105">Отменяет обработку всех выполняемых операций мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-105">Cancels processing for any in-progress media operations.</span></span>

<span data-ttu-id="e4f8a-106">Операции с мультимедиа относятся к IVR операциям [плайпромпт](./call-playprompt.md) и [рекордреспонсе](./call-record.md), которые по умолчанию находятся в очереди на обработку по порядку.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-106">Media operations refer to the IVR operations [playPrompt](./call-playprompt.md) and [recordResponse](./call-record.md), which are by default queued to process in order.</span></span> <span data-ttu-id="e4f8a-107">Метод **канцелмедиапроцессинг** отменяет любую операцию, которая находится в процессе, а также операции, помещенные в очередь.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-107">The **cancelMediaProcessing** method cancels any operation that is in-process as well as operations that are queued.</span></span> <span data-ttu-id="e4f8a-108">Например, этот API можно использовать для очистки очереди операций IVR для новой операции мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-108">For example, this API can be used to clean up the IVR operation queue for a new media operation.</span></span> <span data-ttu-id="e4f8a-109">Тем не менее операция **убскрибетотоне** не будет отменена, так как она работает независимо от очереди операций.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-109">However, it will not cancel a **ubscribeToTone** operation because it operates independent of any operation queue.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4f8a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4f8a-110">Permissions</span></span>
<span data-ttu-id="e4f8a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4f8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4f8a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4f8a-113">Permission type</span></span>                        | <span data-ttu-id="e4f8a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4f8a-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e4f8a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4f8a-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4f8a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-116">Not Supported.</span></span>                              |
| <span data-ttu-id="e4f8a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4f8a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4f8a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-118">Not Supported.</span></span>                              |
| <span data-ttu-id="e4f8a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4f8a-119">Application</span></span>                            | <span data-ttu-id="e4f8a-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-120">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="e4f8a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4f8a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="e4f8a-122">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-122">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e4f8a-123">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-123">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4f8a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4f8a-124">Request headers</span></span>
| <span data-ttu-id="e4f8a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="e4f8a-125">Name</span></span>          | <span data-ttu-id="e4f8a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e4f8a-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e4f8a-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4f8a-127">Authorization</span></span> | <span data-ttu-id="e4f8a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4f8a-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4f8a-130">Content-type</span></span> | <span data-ttu-id="e4f8a-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4f8a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4f8a-133">Request body</span></span>
<span data-ttu-id="e4f8a-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e4f8a-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="e4f8a-135">Parameter</span></span>      | <span data-ttu-id="e4f8a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="e4f8a-136">Type</span></span>    | <span data-ttu-id="e4f8a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="e4f8a-137">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="e4f8a-138">Контекст</span><span class="sxs-lookup"><span data-stu-id="e4f8a-138">clientContext</span></span>  | <span data-ttu-id="e4f8a-139">String</span><span class="sxs-lookup"><span data-stu-id="e4f8a-139">String</span></span>  | <span data-ttu-id="e4f8a-140">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-140">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="e4f8a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4f8a-141">Response</span></span>
<span data-ttu-id="e4f8a-142">В случае успешного выполнения этот метод возвращает `200 OK` код HTTP-ответа и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-142">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="e4f8a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e4f8a-143">Example</span></span>
<span data-ttu-id="e4f8a-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e4f8a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4f8a-145">Request</span></span>
<span data-ttu-id="e4f8a-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e4f8a-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4f8a-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e4f8a-148">C#</span><span class="sxs-lookup"><span data-stu-id="e4f8a-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4f8a-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4f8a-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4f8a-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4f8a-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4f8a-151">Java</span><span class="sxs-lookup"><span data-stu-id="e4f8a-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-cancelmediaprocessing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e4f8a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4f8a-152">Response</span></span>

> <span data-ttu-id="e4f8a-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4f8a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="e4f8a-155">Уведомление — операция отменена для Рекордреспонсе</span><span class="sxs-lookup"><span data-stu-id="e4f8a-155">Notification - Operation canceled for recordResponse</span></span>

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


