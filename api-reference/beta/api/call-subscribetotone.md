---
title: 'Call: Субскрибетотоне'
description: ПодПишитесь на DTMF (многочастотный многочастотный сигнал). Это позволяет получать уведомления, когда пользователь нажимает клавиши на телефоне "тонального".
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f3fe078965877204b767b689ace293c3d4f46a9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461265"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="44830-104">Call: Субскрибетотоне</span><span class="sxs-lookup"><span data-stu-id="44830-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44830-105">ПодПишитесь на DTMF (многочастотный многочастотный сигнал).</span><span class="sxs-lookup"><span data-stu-id="44830-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="44830-106">Это позволяет получать уведомления, когда пользователь нажимает клавиши на "тональном" телефоне.</span><span class="sxs-lookup"><span data-stu-id="44830-106">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="44830-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44830-107">Permissions</span></span>
<span data-ttu-id="44830-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44830-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44830-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44830-110">Permission type</span></span> | <span data-ttu-id="44830-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44830-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="44830-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44830-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="44830-113">Неподдерживаемая функция</span><span class="sxs-lookup"><span data-stu-id="44830-113">Not Supported</span></span>        |
| <span data-ttu-id="44830-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44830-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44830-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="44830-115">Not Supported</span></span>        |
| <span data-ttu-id="44830-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44830-116">Application</span></span>     | <span data-ttu-id="44830-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="44830-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="44830-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44830-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="44830-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44830-119">Request headers</span></span>
| <span data-ttu-id="44830-120">Имя</span><span class="sxs-lookup"><span data-stu-id="44830-120">Name</span></span>          | <span data-ttu-id="44830-121">Описание</span><span class="sxs-lookup"><span data-stu-id="44830-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="44830-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44830-122">Authorization</span></span> | <span data-ttu-id="44830-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44830-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44830-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44830-125">Request body</span></span>
<span data-ttu-id="44830-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="44830-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="44830-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="44830-127">Parameter</span></span>      | <span data-ttu-id="44830-128">Тип</span><span class="sxs-lookup"><span data-stu-id="44830-128">Type</span></span>    | <span data-ttu-id="44830-129">Описание</span><span class="sxs-lookup"><span data-stu-id="44830-129">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="44830-130">Контекст</span><span class="sxs-lookup"><span data-stu-id="44830-130">clientContext</span></span>  | <span data-ttu-id="44830-131">String</span><span class="sxs-lookup"><span data-stu-id="44830-131">String</span></span>  | <span data-ttu-id="44830-132">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="44830-132">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="44830-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="44830-133">Response</span></span>
<span data-ttu-id="44830-134">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="44830-134">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="44830-135">Пример</span><span class="sxs-lookup"><span data-stu-id="44830-135">Example</span></span>
<span data-ttu-id="44830-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="44830-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="44830-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="44830-137">Request</span></span>
<span data-ttu-id="44830-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44830-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="44830-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="44830-139">Response</span></span>

> <span data-ttu-id="44830-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44830-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="44830-142">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="44830-142">Notification - operation completed</span></span>

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
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-subscribetotone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
