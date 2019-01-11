---
title: 'Вызовите: перенаправление'
description: Перенаправление входящего звонка.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: f581a5ce95368e7d852a5b1435ef05bf940f607c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809473"
---
# <a name="call-redirect"></a><span data-ttu-id="674e9-103">Вызовите: перенаправление</span><span class="sxs-lookup"><span data-stu-id="674e9-103">call: redirect</span></span>

> <span data-ttu-id="674e9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="674e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="674e9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="674e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="674e9-106">Перенаправление входящего звонка.</span><span class="sxs-lookup"><span data-stu-id="674e9-106">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="674e9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="674e9-107">Permissions</span></span>
<span data-ttu-id="674e9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="674e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="674e9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="674e9-110">Permission type</span></span> | <span data-ttu-id="674e9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="674e9-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="674e9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="674e9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="674e9-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="674e9-113">Not Supported</span></span>                |
| <span data-ttu-id="674e9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="674e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="674e9-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="674e9-115">Not Supported</span></span>                |
| <span data-ttu-id="674e9-116">Application</span><span class="sxs-lookup"><span data-stu-id="674e9-116">Application</span></span>     | <span data-ttu-id="674e9-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="674e9-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="674e9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="674e9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="674e9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="674e9-119">Request headers</span></span>
| <span data-ttu-id="674e9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="674e9-120">Name</span></span>          | <span data-ttu-id="674e9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="674e9-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="674e9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="674e9-122">Authorization</span></span> | <span data-ttu-id="674e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="674e9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="674e9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="674e9-125">Request body</span></span>
<span data-ttu-id="674e9-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="674e9-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="674e9-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="674e9-127">Parameter</span></span>      | <span data-ttu-id="674e9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="674e9-128">Type</span></span>    |<span data-ttu-id="674e9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="674e9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="674e9-130">целевые значения</span><span class="sxs-lookup"><span data-stu-id="674e9-130">targets</span></span>|<span data-ttu-id="674e9-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="674e9-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="674e9-132">Участники целевой операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="674e9-132">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="674e9-133">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="674e9-133">targetDisposition</span></span>|<span data-ttu-id="674e9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="674e9-134">String</span></span>|<span data-ttu-id="674e9-135">Возможное значение — это:`default`</span><span class="sxs-lookup"><span data-stu-id="674e9-135">The possible value is: `default`</span></span>|
|<span data-ttu-id="674e9-136">timeout</span><span class="sxs-lookup"><span data-stu-id="674e9-136">timeout</span></span>|<span data-ttu-id="674e9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="674e9-137">Int32</span></span>|<span data-ttu-id="674e9-138">Время ожидания в секундах для операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="674e9-138">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="674e9-139">maskCallee</span><span class="sxs-lookup"><span data-stu-id="674e9-139">maskCallee</span></span>|<span data-ttu-id="674e9-140">Логический</span><span class="sxs-lookup"><span data-stu-id="674e9-140">Boolean</span></span>|<span data-ttu-id="674e9-141">Указывает, следует ли скрытие вызываемого абонента.</span><span class="sxs-lookup"><span data-stu-id="674e9-141">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="674e9-142">maskCaller</span><span class="sxs-lookup"><span data-stu-id="674e9-142">maskCaller</span></span>|<span data-ttu-id="674e9-143">Логический</span><span class="sxs-lookup"><span data-stu-id="674e9-143">Boolean</span></span>|<span data-ttu-id="674e9-144">Указывает, следует ли скрытие вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="674e9-144">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="674e9-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="674e9-145">Response</span></span>
<span data-ttu-id="674e9-146">Возвращает `202 Accepted` код ответа</span><span class="sxs-lookup"><span data-stu-id="674e9-146">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="674e9-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="674e9-147">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="674e9-148">Перенаправление звонка</span><span class="sxs-lookup"><span data-stu-id="674e9-148">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="674e9-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="674e9-149">Request</span></span>
<span data-ttu-id="674e9-150">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="674e9-150">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/redirect
Content-Type: application/json
Content-Length: 515

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 99,
  "maskCallee": false,
  "maskCaller": false
}
```

##### <a name="response"></a><span data-ttu-id="674e9-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="674e9-151">Response</span></span>

> <span data-ttu-id="674e9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="674e9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="674e9-154">Переадресация звонка</span><span class="sxs-lookup"><span data-stu-id="674e9-154">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="674e9-155">Уведомления - входящие</span><span class="sxs-lookup"><span data-stu-id="674e9-155">Notification - incoming</span></span>

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
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="674e9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="674e9-156">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/redirect
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 60,
  "maskCallee": false,
  "maskCaller": false
}
```

##### <a name="response"></a><span data-ttu-id="674e9-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="674e9-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="674e9-158">Уведомления — перенаправление</span><span class="sxs-lookup"><span data-stu-id="674e9-158">Notification - redirecting</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "redirecting"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="674e9-159">Уведомления - завершен</span><span class="sxs-lookup"><span data-stu-id="674e9-159">Notification - terminated</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "answeredBy": {
          "identity": {
            "user": {
              "displayName": "Test User 2",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
            }
          }
        },
        "terminationReason": "AppRedirected"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
