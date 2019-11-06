---
title: 'Call: Канцелмедиапроцессинг'
description: Отменяет обработку мультимедиа для всех выполняемых операций Плайпромпт или записи.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1463489c82d1595e1bdcaa9629e5f306b95aa19f
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006363"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="55aa9-103">Call: Канцелмедиапроцессинг</span><span class="sxs-lookup"><span data-stu-id="55aa9-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55aa9-104">Отменяет обработку мультимедиа для всех выполняемых операций Плайпромпт или записи.</span><span class="sxs-lookup"><span data-stu-id="55aa9-104">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="55aa9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55aa9-105">Permissions</span></span>
<span data-ttu-id="55aa9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55aa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55aa9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55aa9-108">Permission type</span></span>                        | <span data-ttu-id="55aa9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55aa9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="55aa9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55aa9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="55aa9-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55aa9-111">Not Supported.</span></span>                              |
| <span data-ttu-id="55aa9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55aa9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55aa9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55aa9-113">Not Supported.</span></span>                              |
| <span data-ttu-id="55aa9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55aa9-114">Application</span></span>                            | <span data-ttu-id="55aa9-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="55aa9-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="55aa9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55aa9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /communications/calls/{id}/cancelMediaProcessing
```
> <span data-ttu-id="55aa9-117">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="55aa9-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="55aa9-118">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="55aa9-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55aa9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55aa9-119">Request headers</span></span>
| <span data-ttu-id="55aa9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="55aa9-120">Name</span></span>          | <span data-ttu-id="55aa9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="55aa9-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="55aa9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55aa9-122">Authorization</span></span> | <span data-ttu-id="55aa9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55aa9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55aa9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55aa9-125">Request body</span></span>
<span data-ttu-id="55aa9-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="55aa9-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55aa9-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="55aa9-127">Parameter</span></span>      | <span data-ttu-id="55aa9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="55aa9-128">Type</span></span>    | <span data-ttu-id="55aa9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="55aa9-129">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="55aa9-130">ко</span><span class="sxs-lookup"><span data-stu-id="55aa9-130">all</span></span>            | <span data-ttu-id="55aa9-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="55aa9-131">Boolean</span></span> | <span data-ttu-id="55aa9-132">Флаг, указывающий, следует ли остановить все операции или текущие.</span><span class="sxs-lookup"><span data-stu-id="55aa9-132">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="55aa9-133">Контекст</span><span class="sxs-lookup"><span data-stu-id="55aa9-133">clientContext</span></span>  | <span data-ttu-id="55aa9-134">String</span><span class="sxs-lookup"><span data-stu-id="55aa9-134">String</span></span>  | <span data-ttu-id="55aa9-135">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="55aa9-135">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="55aa9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="55aa9-136">Response</span></span>
<span data-ttu-id="55aa9-137">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="55aa9-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="55aa9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="55aa9-138">Example</span></span>
<span data-ttu-id="55aa9-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="55aa9-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="55aa9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="55aa9-140">Request</span></span>
<span data-ttu-id="55aa9-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55aa9-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="55aa9-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="55aa9-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "all": true,
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="55aa9-143">C#</span><span class="sxs-lookup"><span data-stu-id="55aa9-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55aa9-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55aa9-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55aa9-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55aa9-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55aa9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="55aa9-146">Response</span></span>

> <span data-ttu-id="55aa9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55aa9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "running",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="55aa9-149">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="55aa9-149">Notification - operation completed</span></span>

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
        "@odata.type": "#microsoft.graph.commsOperation",
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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
