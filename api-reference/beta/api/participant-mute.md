---
title: 'Участник: Выкл.'
description: Отключение микрофона определенного участника в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d41d97556aff7093660c0cdfb75a43f8b862c0d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964475"
---
# <a name="participant-mute"></a><span data-ttu-id="f58b2-103">Участник: Выкл.</span><span class="sxs-lookup"><span data-stu-id="f58b2-103">participant: mute</span></span>

> <span data-ttu-id="f58b2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f58b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f58b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f58b2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f58b2-106">Отключение микрофона определенного участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="f58b2-106">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="f58b2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f58b2-107">Permissions</span></span>
<span data-ttu-id="f58b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f58b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f58b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f58b2-110">Permission type</span></span> | <span data-ttu-id="f58b2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f58b2-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="f58b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f58b2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f58b2-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f58b2-113">Not Supported</span></span>        |
| <span data-ttu-id="f58b2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f58b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f58b2-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f58b2-115">Not Supported</span></span>        |
| <span data-ttu-id="f58b2-116">Application</span><span class="sxs-lookup"><span data-stu-id="f58b2-116">Application</span></span>     | <span data-ttu-id="f58b2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f58b2-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="f58b2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f58b2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="f58b2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f58b2-119">Request headers</span></span>
| <span data-ttu-id="f58b2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f58b2-120">Name</span></span>          | <span data-ttu-id="f58b2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f58b2-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f58b2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f58b2-122">Authorization</span></span> | <span data-ttu-id="f58b2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f58b2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f58b2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f58b2-125">Request body</span></span>
<span data-ttu-id="f58b2-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f58b2-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f58b2-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="f58b2-127">Parameter</span></span>      | <span data-ttu-id="f58b2-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f58b2-128">Type</span></span>    |<span data-ttu-id="f58b2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f58b2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f58b2-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="f58b2-130">clientContext</span></span>|<span data-ttu-id="f58b2-131">Строка</span><span class="sxs-lookup"><span data-stu-id="f58b2-131">String</span></span>|<span data-ttu-id="f58b2-132">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="f58b2-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="f58b2-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f58b2-133">Response</span></span>
<span data-ttu-id="f58b2-134">Успешно завершена, этот метод возвращает `200 OK` объект [commsOperation](../resources/commsoperation.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f58b2-134">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f58b2-135">Пример</span><span class="sxs-lookup"><span data-stu-id="f58b2-135">Example</span></span>
<span data-ttu-id="f58b2-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f58b2-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f58b2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f58b2-137">Request</span></span>
<span data-ttu-id="f58b2-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f58b2-138">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="f58b2-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="f58b2-139">Response</span></span>

> <span data-ttu-id="f58b2-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f58b2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

## <a name="example---mute-specific-participant"></a><span data-ttu-id="f58b2-142">Пример — отключить определенного участника</span><span class="sxs-lookup"><span data-stu-id="f58b2-142">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="f58b2-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="f58b2-143">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="f58b2-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="f58b2-144">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="f58b2-145">Выключен ли уведомления - участников, добавлены участника</span><span class="sxs-lookup"><span data-stu-id="f58b2-145">Notification - roster updated with participant muted</span></span>

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
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "0698446E77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "123456W77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
