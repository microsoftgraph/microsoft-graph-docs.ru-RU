---
title: 'Участник: configureMixer'
description: Настройка как смешанное аудио для различных участников в многосторонней беседе.
ms.openlocfilehash: 58ccdcb345d55ae28b30dd5ded6b95ef5b30fe81
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156003"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="db193-103">Участник: configureMixer</span><span class="sxs-lookup"><span data-stu-id="db193-103">participant: configureMixer</span></span>

> <span data-ttu-id="db193-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db193-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db193-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db193-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db193-106">Настройка как смешанное аудио для различных участников в многосторонней беседе.</span><span class="sxs-lookup"><span data-stu-id="db193-106">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="db193-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db193-107">Permissions</span></span>
<span data-ttu-id="db193-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db193-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db193-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db193-110">Permission type</span></span> | <span data-ttu-id="db193-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db193-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="db193-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db193-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="db193-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db193-113">Not Supported</span></span>        |
| <span data-ttu-id="db193-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db193-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db193-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db193-115">Not Supported</span></span>        |
| <span data-ttu-id="db193-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="db193-116">Application</span></span>     | <span data-ttu-id="db193-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="db193-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db193-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db193-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="db193-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db193-119">Request headers</span></span>
| <span data-ttu-id="db193-120">Имя</span><span class="sxs-lookup"><span data-stu-id="db193-120">Name</span></span>          | <span data-ttu-id="db193-121">Описание</span><span class="sxs-lookup"><span data-stu-id="db193-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="db193-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db193-122">Authorization</span></span> | <span data-ttu-id="db193-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db193-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db193-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db193-125">Request body</span></span>
<span data-ttu-id="db193-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="db193-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="db193-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="db193-127">Parameter</span></span>      | <span data-ttu-id="db193-128">Тип</span><span class="sxs-lookup"><span data-stu-id="db193-128">Type</span></span>    |<span data-ttu-id="db193-129">Описание</span><span class="sxs-lookup"><span data-stu-id="db193-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db193-130">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="db193-130">participantMixerLevels</span></span>|<span data-ttu-id="db193-131">[participantMixerLevel](../resources/participantmixerlevel.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="db193-131">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="db193-132">Конфигурация микшер уровни для заданного звука участников.</span><span class="sxs-lookup"><span data-stu-id="db193-132">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="db193-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="db193-133">clientContext</span></span>|<span data-ttu-id="db193-134">String</span><span class="sxs-lookup"><span data-stu-id="db193-134">String</span></span>|<span data-ttu-id="db193-135">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="db193-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="db193-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db193-136">Response</span></span>
<span data-ttu-id="db193-137">Возвращает `202 Accepted` код ответа и расположения заголовком с uri для [commsOperation](../resources/commsoperation.md) , созданные для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="db193-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="db193-138">Пример</span><span class="sxs-lookup"><span data-stu-id="db193-138">Example</span></span>
<span data-ttu-id="db193-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="db193-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="db193-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="db193-140">Request</span></span>
<span data-ttu-id="db193-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db193-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "participant_configureMixer"
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

##### <a name="response"></a><span data-ttu-id="db193-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="db193-142">Response</span></span>

> <span data-ttu-id="db193-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db193-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="db193-145">Уведомления - операция завершена</span><span class="sxs-lookup"><span data-stu-id="db193-145">Notification - operation completed</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
