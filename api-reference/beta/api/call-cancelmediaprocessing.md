---
title: 'Call: Канцелмедиапроцессинг'
description: Отменяет обработку мультимедиа для всех выполняемых операций Плайпромпт или записи.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 53f19060fd2c0d6e388f9d3efe1626750a0df4a3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438806"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="3a900-103">Call: Канцелмедиапроцессинг</span><span class="sxs-lookup"><span data-stu-id="3a900-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a900-104">Отменяет обработку мультимедиа для всех выполняемых операций Плайпромпт или записи.</span><span class="sxs-lookup"><span data-stu-id="3a900-104">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a900-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a900-105">Permissions</span></span>
<span data-ttu-id="3a900-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a900-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a900-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a900-108">Permission type</span></span>                        | <span data-ttu-id="3a900-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a900-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3a900-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a900-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a900-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a900-111">Not Supported.</span></span>                              |
| <span data-ttu-id="3a900-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a900-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a900-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a900-113">Not Supported.</span></span>                              |
| <span data-ttu-id="3a900-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a900-114">Application</span></span>                            | <span data-ttu-id="3a900-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3a900-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="3a900-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a900-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="3a900-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a900-117">Request headers</span></span>
| <span data-ttu-id="3a900-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3a900-118">Name</span></span>          | <span data-ttu-id="3a900-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3a900-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3a900-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a900-120">Authorization</span></span> | <span data-ttu-id="3a900-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a900-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a900-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a900-123">Request body</span></span>
<span data-ttu-id="3a900-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3a900-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a900-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="3a900-125">Parameter</span></span>      | <span data-ttu-id="3a900-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3a900-126">Type</span></span>    | <span data-ttu-id="3a900-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3a900-127">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="3a900-128">ко</span><span class="sxs-lookup"><span data-stu-id="3a900-128">all</span></span>            | <span data-ttu-id="3a900-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a900-129">Boolean</span></span> | <span data-ttu-id="3a900-130">Флаг, указывающий, следует ли остановить все операции или текущие.</span><span class="sxs-lookup"><span data-stu-id="3a900-130">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="3a900-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="3a900-131">clientContext</span></span>  | <span data-ttu-id="3a900-132">String</span><span class="sxs-lookup"><span data-stu-id="3a900-132">String</span></span>  | <span data-ttu-id="3a900-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="3a900-133">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="3a900-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a900-134">Response</span></span>
<span data-ttu-id="3a900-135">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="3a900-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="3a900-136">Пример</span><span class="sxs-lookup"><span data-stu-id="3a900-136">Example</span></span>
<span data-ttu-id="3a900-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3a900-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3a900-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a900-138">Request</span></span>
<span data-ttu-id="3a900-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a900-139">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3a900-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a900-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "all": true,
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3a900-141">C#</span><span class="sxs-lookup"><span data-stu-id="3a900-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-cancelmediaprocessing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a900-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="3a900-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-cancelmediaprocessing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3a900-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3a900-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-cancelmediaprocessing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3a900-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a900-144">Response</span></span>

> <span data-ttu-id="3a900-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a900-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="3a900-147">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="3a900-147">Notification - operation completed</span></span>

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
        "@odata.type": "#microsoft.graph.commsOperation",
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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
