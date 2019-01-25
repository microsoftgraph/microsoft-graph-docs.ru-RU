---
title: 'вызов: playPrompt'
description: Воспроизведение запрос в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32ea1b838a71d40a6f6106a648962c6a77c29057
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507791"
---
# <a name="call-playprompt"></a><span data-ttu-id="9547c-103">вызов: playPrompt</span><span class="sxs-lookup"><span data-stu-id="9547c-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9547c-104">Воспроизведение запрос в вызове.</span><span class="sxs-lookup"><span data-stu-id="9547c-104">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="9547c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9547c-105">Permissions</span></span>
<span data-ttu-id="9547c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9547c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9547c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9547c-108">Permission type</span></span>                        | <span data-ttu-id="9547c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9547c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9547c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9547c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9547c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9547c-111">Not Supported.</span></span>                               |
| <span data-ttu-id="9547c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9547c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9547c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9547c-113">Not Supported.</span></span>                               |
| <span data-ttu-id="9547c-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="9547c-114">Application</span></span>                            | <span data-ttu-id="9547c-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9547c-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="9547c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9547c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="9547c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9547c-117">Request headers</span></span>
| <span data-ttu-id="9547c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9547c-118">Name</span></span>          | <span data-ttu-id="9547c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9547c-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9547c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9547c-120">Authorization</span></span> | <span data-ttu-id="9547c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9547c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9547c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9547c-123">Request body</span></span>
<span data-ttu-id="9547c-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9547c-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9547c-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="9547c-125">Parameter</span></span>      | <span data-ttu-id="9547c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9547c-126">Type</span></span>    |<span data-ttu-id="9547c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9547c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9547c-128">запросы</span><span class="sxs-lookup"><span data-stu-id="9547c-128">prompts</span></span>|<span data-ttu-id="9547c-129">[запрос](../resources/prompt.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="9547c-129">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="9547c-130">ClientContext</span><span class="sxs-lookup"><span data-stu-id="9547c-130">clientContext</span></span>|<span data-ttu-id="9547c-131">String</span><span class="sxs-lookup"><span data-stu-id="9547c-131">String</span></span>|<span data-ttu-id="9547c-132">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="9547c-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="9547c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9547c-133">Response</span></span>
<span data-ttu-id="9547c-134">Успешно завершена, этот метод возвращает `200 OK` объект [playPromptOperation](../resources/playPromptOperation.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9547c-134">If successful, this method returns `200 OK` response code and [playPromptOperation](../resources/playPromptOperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9547c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="9547c-135">Example</span></span>
<span data-ttu-id="9547c-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9547c-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9547c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9547c-137">Request</span></span>
<span data-ttu-id="9547c-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9547c-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      "loop": 5
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="9547c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="9547c-139">Response</span></span>

> <span data-ttu-id="9547c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9547c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="9547c-142">Уведомления - операция завершена</span><span class="sxs-lookup"><span data-stu-id="9547c-142">Notification - operation completed</span></span>

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
    "Error: /api-reference/beta/api/call-playprompt.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
