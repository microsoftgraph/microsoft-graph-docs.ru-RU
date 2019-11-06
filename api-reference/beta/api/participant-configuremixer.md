---
title: 'участник: Конфигуремиксер'
description: Настройка смешанного звука для разных участников многочастной беседы.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c59c56c7c862a62247cadf8472a042e3ea8d9af2
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006482"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="31bb1-103">участник: Конфигуремиксер</span><span class="sxs-lookup"><span data-stu-id="31bb1-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31bb1-104">Настройка смешанного звука для разных участников многочастной беседы.</span><span class="sxs-lookup"><span data-stu-id="31bb1-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="31bb1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31bb1-105">Permissions</span></span>
<span data-ttu-id="31bb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31bb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31bb1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31bb1-108">Permission type</span></span> | <span data-ttu-id="31bb1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31bb1-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="31bb1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31bb1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="31bb1-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31bb1-111">Not Supported</span></span>        |
| <span data-ttu-id="31bb1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31bb1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31bb1-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31bb1-113">Not Supported</span></span>        |
| <span data-ttu-id="31bb1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31bb1-114">Application</span></span>     | <span data-ttu-id="31bb1-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="31bb1-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31bb1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31bb1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /communications/calls/{id}/participants/configureMixer
```
> <span data-ttu-id="31bb1-117">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="31bb1-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="31bb1-118">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="31bb1-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31bb1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31bb1-119">Request headers</span></span>
| <span data-ttu-id="31bb1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="31bb1-120">Name</span></span>          | <span data-ttu-id="31bb1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="31bb1-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="31bb1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31bb1-122">Authorization</span></span> | <span data-ttu-id="31bb1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31bb1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31bb1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31bb1-125">Request body</span></span>
<span data-ttu-id="31bb1-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="31bb1-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="31bb1-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="31bb1-127">Parameter</span></span>      | <span data-ttu-id="31bb1-128">Тип</span><span class="sxs-lookup"><span data-stu-id="31bb1-128">Type</span></span>    |<span data-ttu-id="31bb1-129">Описание</span><span class="sxs-lookup"><span data-stu-id="31bb1-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31bb1-130">партиЦипантмиксерлевелс</span><span class="sxs-lookup"><span data-stu-id="31bb1-130">participantMixerLevels</span></span>|<span data-ttu-id="31bb1-131">Коллекция [партиЦипантмиксерлевел](../resources/participantmixerlevel.md)</span><span class="sxs-lookup"><span data-stu-id="31bb1-131">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="31bb1-132">Настройка уровней микшера для данного участника аудио.</span><span class="sxs-lookup"><span data-stu-id="31bb1-132">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="31bb1-133">Контекст</span><span class="sxs-lookup"><span data-stu-id="31bb1-133">clientContext</span></span>|<span data-ttu-id="31bb1-134">String</span><span class="sxs-lookup"><span data-stu-id="31bb1-134">String</span></span>|<span data-ttu-id="31bb1-135">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="31bb1-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="31bb1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="31bb1-136">Response</span></span>
<span data-ttu-id="31bb1-137">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="31bb1-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="31bb1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="31bb1-138">Example</span></span>
<span data-ttu-id="31bb1-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="31bb1-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="31bb1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="31bb1-140">Request</span></span>
<span data-ttu-id="31bb1-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31bb1-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="31bb1-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="31bb1-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="31bb1-143">C#</span><span class="sxs-lookup"><span data-stu-id="31bb1-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-configuremixer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31bb1-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31bb1-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-configuremixer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="31bb1-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31bb1-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-configuremixer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="31bb1-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="31bb1-146">Response</span></span>

> <span data-ttu-id="31bb1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31bb1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
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

##### <a name="notification---operation-completed"></a><span data-ttu-id="31bb1-149">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="31bb1-149">Notification - operation completed</span></span>

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
