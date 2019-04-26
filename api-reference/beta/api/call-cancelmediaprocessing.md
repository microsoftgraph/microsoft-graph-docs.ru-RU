---
title: 'Call: Канцелмедиапроцессинг'
description: ОтМеняет обработку мультимедиа для всех выполняемых операций Плайпромпт или записи.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 28637d3544b3b7d0e6c5756661e2b5b1eff31e0b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328137"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="98f49-103">Call: Канцелмедиапроцессинг</span><span class="sxs-lookup"><span data-stu-id="98f49-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98f49-104">ОтМеняет обработку мультимедиа для всех выполняемых операций Плайпромпт или записи.</span><span class="sxs-lookup"><span data-stu-id="98f49-104">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="98f49-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98f49-105">Permissions</span></span>
<span data-ttu-id="98f49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98f49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98f49-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98f49-108">Permission type</span></span>                        | <span data-ttu-id="98f49-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98f49-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98f49-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98f49-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="98f49-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98f49-111">Not Supported.</span></span>                              |
| <span data-ttu-id="98f49-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98f49-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98f49-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98f49-113">Not Supported.</span></span>                              |
| <span data-ttu-id="98f49-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="98f49-114">Application</span></span>                            | <span data-ttu-id="98f49-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="98f49-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="98f49-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98f49-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="98f49-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98f49-117">Request headers</span></span>
| <span data-ttu-id="98f49-118">Имя</span><span class="sxs-lookup"><span data-stu-id="98f49-118">Name</span></span>          | <span data-ttu-id="98f49-119">Описание</span><span class="sxs-lookup"><span data-stu-id="98f49-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="98f49-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98f49-120">Authorization</span></span> | <span data-ttu-id="98f49-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98f49-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98f49-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98f49-123">Request body</span></span>
<span data-ttu-id="98f49-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="98f49-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="98f49-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="98f49-125">Parameter</span></span>      | <span data-ttu-id="98f49-126">Тип</span><span class="sxs-lookup"><span data-stu-id="98f49-126">Type</span></span>    | <span data-ttu-id="98f49-127">Описание</span><span class="sxs-lookup"><span data-stu-id="98f49-127">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="98f49-128">ко</span><span class="sxs-lookup"><span data-stu-id="98f49-128">all</span></span>            | <span data-ttu-id="98f49-129">Логический</span><span class="sxs-lookup"><span data-stu-id="98f49-129">Boolean</span></span> | <span data-ttu-id="98f49-130">Флаг, указывающий, следует ли остановить все операции или текущие.</span><span class="sxs-lookup"><span data-stu-id="98f49-130">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="98f49-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="98f49-131">clientContext</span></span>  | <span data-ttu-id="98f49-132">String</span><span class="sxs-lookup"><span data-stu-id="98f49-132">String</span></span>  | <span data-ttu-id="98f49-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="98f49-133">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="98f49-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="98f49-134">Response</span></span>
<span data-ttu-id="98f49-135">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="98f49-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="98f49-136">Пример</span><span class="sxs-lookup"><span data-stu-id="98f49-136">Example</span></span>
<span data-ttu-id="98f49-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="98f49-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="98f49-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="98f49-138">Request</span></span>
<span data-ttu-id="98f49-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98f49-139">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="98f49-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="98f49-140">Response</span></span>

> <span data-ttu-id="98f49-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98f49-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="98f49-143">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="98f49-143">Notification - operation completed</span></span>

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
  "suppressions": []
}
-->
