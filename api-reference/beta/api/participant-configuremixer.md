---
title: 'Участник: configureMixer'
description: Настройка как смешанное аудио для различных участников в многосторонней беседе.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0be23ec4c9e7835c919328655e89880003546472
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530043"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="58ab1-103">Участник: configureMixer</span><span class="sxs-lookup"><span data-stu-id="58ab1-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58ab1-104">Настройка как смешанное аудио для различных участников в многосторонней беседе.</span><span class="sxs-lookup"><span data-stu-id="58ab1-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="58ab1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58ab1-105">Permissions</span></span>
<span data-ttu-id="58ab1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58ab1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58ab1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58ab1-108">Permission type</span></span> | <span data-ttu-id="58ab1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58ab1-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="58ab1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58ab1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="58ab1-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="58ab1-111">Not Supported</span></span>        |
| <span data-ttu-id="58ab1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58ab1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58ab1-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="58ab1-113">Not Supported</span></span>        |
| <span data-ttu-id="58ab1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58ab1-114">Application</span></span>     | <span data-ttu-id="58ab1-115">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="58ab1-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58ab1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58ab1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="58ab1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58ab1-117">Request headers</span></span>
| <span data-ttu-id="58ab1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="58ab1-118">Name</span></span>          | <span data-ttu-id="58ab1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="58ab1-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="58ab1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58ab1-120">Authorization</span></span> | <span data-ttu-id="58ab1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58ab1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58ab1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58ab1-123">Request body</span></span>
<span data-ttu-id="58ab1-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="58ab1-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58ab1-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="58ab1-125">Parameter</span></span>      | <span data-ttu-id="58ab1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="58ab1-126">Type</span></span>    |<span data-ttu-id="58ab1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="58ab1-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58ab1-128">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="58ab1-128">participantMixerLevels</span></span>|<span data-ttu-id="58ab1-129">[participantMixerLevel](../resources/participantmixerlevel.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="58ab1-129">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="58ab1-130">Конфигурация микшер уровни для заданного звука участников.</span><span class="sxs-lookup"><span data-stu-id="58ab1-130">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="58ab1-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="58ab1-131">clientContext</span></span>|<span data-ttu-id="58ab1-132">String</span><span class="sxs-lookup"><span data-stu-id="58ab1-132">String</span></span>|<span data-ttu-id="58ab1-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="58ab1-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="58ab1-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="58ab1-134">Response</span></span>
<span data-ttu-id="58ab1-135">Возвращает `202 Accepted` код ответа и расположения заголовком с uri для [commsOperation](../resources/commsoperation.md) , созданные для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="58ab1-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="58ab1-136">Пример</span><span class="sxs-lookup"><span data-stu-id="58ab1-136">Example</span></span>
<span data-ttu-id="58ab1-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="58ab1-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="58ab1-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="58ab1-138">Request</span></span>
<span data-ttu-id="58ab1-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58ab1-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "participant-configureMixer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/configureMixer
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

##### <a name="response"></a><span data-ttu-id="58ab1-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="58ab1-140">Response</span></span>

> <span data-ttu-id="58ab1-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58ab1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="58ab1-143">Уведомления - операция завершена</span><span class="sxs-lookup"><span data-stu-id="58ab1-143">Notification - operation completed</span></span>

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
    "Error: /api-reference/beta/api/participant-configuremixer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
