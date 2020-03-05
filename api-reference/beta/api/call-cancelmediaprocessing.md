---
title: 'Call: Канцелмедиапроцессинг'
description: Отменяет обработку мультимедиа для всех выполняющихся операций Плайпромпт или Рекордреспонсе.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0f9ec0eaede3383d6e99a05e4aa4023dd914d9b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440887"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="03663-103">Call: Канцелмедиапроцессинг</span><span class="sxs-lookup"><span data-stu-id="03663-103">call: cancelMediaProcessing</span></span>

<span data-ttu-id="03663-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="03663-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03663-105">Отменяет обработку всех выполняемых [приглашений на проигрывание](./call-playprompt.md) или [запись отклика](./call-record.md) .</span><span class="sxs-lookup"><span data-stu-id="03663-105">Cancels processing for any in-progress [play prompt](./call-playprompt.md) or [record response](./call-record.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="03663-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03663-106">Permissions</span></span>
<span data-ttu-id="03663-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03663-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03663-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03663-109">Permission type</span></span>                        | <span data-ttu-id="03663-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03663-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03663-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03663-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="03663-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03663-112">Not Supported.</span></span>                              |
| <span data-ttu-id="03663-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03663-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03663-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03663-114">Not Supported.</span></span>                              |
| <span data-ttu-id="03663-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03663-115">Application</span></span>                            | <span data-ttu-id="03663-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="03663-116">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="03663-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03663-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="03663-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="03663-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="03663-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="03663-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03663-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03663-120">Request headers</span></span>
| <span data-ttu-id="03663-121">Имя</span><span class="sxs-lookup"><span data-stu-id="03663-121">Name</span></span>          | <span data-ttu-id="03663-122">Описание</span><span class="sxs-lookup"><span data-stu-id="03663-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="03663-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03663-123">Authorization</span></span> | <span data-ttu-id="03663-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03663-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03663-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03663-126">Content-type</span></span> | <span data-ttu-id="03663-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03663-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03663-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03663-129">Request body</span></span>
<span data-ttu-id="03663-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="03663-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03663-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="03663-131">Parameter</span></span>      | <span data-ttu-id="03663-132">Тип</span><span class="sxs-lookup"><span data-stu-id="03663-132">Type</span></span>    | <span data-ttu-id="03663-133">Описание</span><span class="sxs-lookup"><span data-stu-id="03663-133">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="03663-134">Контекст</span><span class="sxs-lookup"><span data-stu-id="03663-134">clientContext</span></span>  | <span data-ttu-id="03663-135">String</span><span class="sxs-lookup"><span data-stu-id="03663-135">String</span></span>  | <span data-ttu-id="03663-136">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="03663-136">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="03663-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="03663-137">Response</span></span>
<span data-ttu-id="03663-138">В случае успешного выполнения этот метод возвращает `200 OK` код HTTP-ответа и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="03663-138">If successful, this method returns a `200 OK` HTTP response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="03663-139">Пример</span><span class="sxs-lookup"><span data-stu-id="03663-139">Example</span></span>
<span data-ttu-id="03663-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="03663-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="03663-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="03663-141">Request</span></span>
<span data-ttu-id="03663-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03663-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03663-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="03663-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="03663-144">C#</span><span class="sxs-lookup"><span data-stu-id="03663-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03663-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03663-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03663-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03663-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="03663-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="03663-147">Response</span></span>

> <span data-ttu-id="03663-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03663-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-canceled-for-recordresponse"></a><span data-ttu-id="03663-150">Уведомление — операция отменена для Рекордреспонсе</span><span class="sxs-lookup"><span data-stu-id="03663-150">Notification - Operation canceled for recordResponse</span></span>

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
          "message": "Action falied, the operation was cancelled."
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
