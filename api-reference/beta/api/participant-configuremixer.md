---
title: 'участник: configureMixer'
description: Настройка смешанного звука для разных участников многопартийного разговора.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d9b8efa45be5163e088bef06e2d71959e80cae58
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037916"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="d3850-103">участник: configureMixer</span><span class="sxs-lookup"><span data-stu-id="d3850-103">participant: configureMixer</span></span>

<span data-ttu-id="d3850-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3850-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3850-105">Настройка смешанного звука для разных участников многопартийного разговора.</span><span class="sxs-lookup"><span data-stu-id="d3850-105">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3850-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3850-106">Permissions</span></span>
<span data-ttu-id="d3850-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3850-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3850-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3850-109">Permission type</span></span> | <span data-ttu-id="d3850-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3850-110">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="d3850-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3850-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3850-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3850-112">Not Supported</span></span>        |
| <span data-ttu-id="d3850-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3850-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3850-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3850-114">Not Supported</span></span>        |
| <span data-ttu-id="d3850-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3850-115">Application</span></span>     | <span data-ttu-id="d3850-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="d3850-116">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3850-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3850-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /communications/calls/{id}/participants/configureMixer
```
> <span data-ttu-id="d3850-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="d3850-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d3850-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="d3850-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3850-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3850-120">Request headers</span></span>
| <span data-ttu-id="d3850-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d3850-121">Name</span></span>          | <span data-ttu-id="d3850-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d3850-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d3850-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3850-123">Authorization</span></span> | <span data-ttu-id="d3850-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3850-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3850-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3850-126">Request body</span></span>
<span data-ttu-id="d3850-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d3850-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3850-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="d3850-128">Parameter</span></span>      | <span data-ttu-id="d3850-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d3850-129">Type</span></span>    |<span data-ttu-id="d3850-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d3850-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3850-131">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="d3850-131">participantMixerLevels</span></span>|<span data-ttu-id="d3850-132">[коллекция participantMixerLevel](../resources/participantmixerlevel.md)</span><span class="sxs-lookup"><span data-stu-id="d3850-132">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="d3850-133">Конфигурация уровней микшера для данного звукового участника.</span><span class="sxs-lookup"><span data-stu-id="d3850-133">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="d3850-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="d3850-134">clientContext</span></span>|<span data-ttu-id="d3850-135">String</span><span class="sxs-lookup"><span data-stu-id="d3850-135">String</span></span>|<span data-ttu-id="d3850-136">Клиентский контекст.</span><span class="sxs-lookup"><span data-stu-id="d3850-136">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="d3850-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3850-137">Response</span></span>
<span data-ttu-id="d3850-138">Возвращает `202 Accepted` код ответа и заглавную ссылку Location с uri в [commsOperation,](../resources/commsoperation.md) созданный для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="d3850-138">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="d3850-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d3850-139">Example</span></span>
<span data-ttu-id="d3850-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d3850-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d3850-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3850-141">Request</span></span>
<span data-ttu-id="d3850-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3850-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d3850-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3850-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-configureMixer"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/configureMixer
Content-Type: application/json
Content-Length: 501

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "participantMixerLevels": [
    {
      "participant": "550fae72-d251-43ec-868c-373732c2704f",
      "exclusive": true,
      "ducking": {
        "rampActive": 50,
        "rampInactive": 50,
        "lowerLevel": 10,
        "upperLevel": 50
      },
      "sourceLevels": [
        {
          "participant": "632899f8-2ea1-4604-8413-27bd2892079f",
          "level": 50,
          "duckOthers": false
        }
      ]
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d3850-144">C#</span><span class="sxs-lookup"><span data-stu-id="d3850-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-configuremixer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3850-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3850-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-configuremixer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3850-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3850-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-configuremixer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d3850-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3850-147">Response</span></span>

> <span data-ttu-id="d3850-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3850-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "participant-configureMixer",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.commsOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "running"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="d3850-149">Уведомление — операция завершена</span><span class="sxs-lookup"><span data-stu-id="d3850-149">Notification - operation completed</span></span>

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
      "@odata.type": "#microsoft.graph.commsOperation",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5",
        "@odata.etag": "W/\"1\"",
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
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


