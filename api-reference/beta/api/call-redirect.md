---
title: 'Вызовите: перенаправление'
description: Перенаправление входящего звонка.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6a926aa082cc35896d11ec4124091b0d2c838c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511991"
---
# <a name="call-redirect"></a><span data-ttu-id="a8ce0-103">Вызовите: перенаправление</span><span class="sxs-lookup"><span data-stu-id="a8ce0-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8ce0-104">Перенаправление входящего звонка.</span><span class="sxs-lookup"><span data-stu-id="a8ce0-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8ce0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8ce0-105">Permissions</span></span>
<span data-ttu-id="a8ce0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8ce0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8ce0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8ce0-108">Permission type</span></span> | <span data-ttu-id="a8ce0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8ce0-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="a8ce0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8ce0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8ce0-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a8ce0-111">Not Supported</span></span>                |
| <span data-ttu-id="a8ce0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8ce0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8ce0-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a8ce0-113">Not Supported</span></span>                |
| <span data-ttu-id="a8ce0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8ce0-114">Application</span></span>     | <span data-ttu-id="a8ce0-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="a8ce0-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="a8ce0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8ce0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="a8ce0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8ce0-117">Request headers</span></span>
| <span data-ttu-id="a8ce0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a8ce0-118">Name</span></span>          | <span data-ttu-id="a8ce0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ce0-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a8ce0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8ce0-120">Authorization</span></span> | <span data-ttu-id="a8ce0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8ce0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8ce0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8ce0-123">Request body</span></span>
<span data-ttu-id="a8ce0-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a8ce0-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8ce0-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="a8ce0-125">Parameter</span></span>      | <span data-ttu-id="a8ce0-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a8ce0-126">Type</span></span>    |<span data-ttu-id="a8ce0-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ce0-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8ce0-128">Targets</span><span class="sxs-lookup"><span data-stu-id="a8ce0-128">targets</span></span>|<span data-ttu-id="a8ce0-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a8ce0-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="a8ce0-130">Участники целевой операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="a8ce0-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="a8ce0-131">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="a8ce0-131">targetDisposition</span></span>|<span data-ttu-id="a8ce0-132">String</span><span class="sxs-lookup"><span data-stu-id="a8ce0-132">String</span></span>|<span data-ttu-id="a8ce0-133">Возможное значение — это:`default`</span><span class="sxs-lookup"><span data-stu-id="a8ce0-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="a8ce0-134">timeout</span><span class="sxs-lookup"><span data-stu-id="a8ce0-134">timeout</span></span>|<span data-ttu-id="a8ce0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a8ce0-135">Int32</span></span>|<span data-ttu-id="a8ce0-136">Время ожидания в секундах для операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="a8ce0-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="a8ce0-137">maskCallee</span><span class="sxs-lookup"><span data-stu-id="a8ce0-137">maskCallee</span></span>|<span data-ttu-id="a8ce0-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="a8ce0-138">Boolean</span></span>|<span data-ttu-id="a8ce0-139">Указывает, следует ли скрытие вызываемого абонента.</span><span class="sxs-lookup"><span data-stu-id="a8ce0-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="a8ce0-140">maskCaller</span><span class="sxs-lookup"><span data-stu-id="a8ce0-140">maskCaller</span></span>|<span data-ttu-id="a8ce0-141">Логическое</span><span class="sxs-lookup"><span data-stu-id="a8ce0-141">Boolean</span></span>|<span data-ttu-id="a8ce0-142">Указывает, следует ли скрытие вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="a8ce0-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="a8ce0-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8ce0-143">Response</span></span>
<span data-ttu-id="a8ce0-144">Возвращает `202 Accepted` код ответа</span><span class="sxs-lookup"><span data-stu-id="a8ce0-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="a8ce0-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="a8ce0-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="a8ce0-146">Перенаправление звонка</span><span class="sxs-lookup"><span data-stu-id="a8ce0-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="a8ce0-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8ce0-147">Request</span></span>
<span data-ttu-id="a8ce0-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8ce0-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="a8ce0-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8ce0-149">Response</span></span>

> <span data-ttu-id="a8ce0-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8ce0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="a8ce0-152">Переадресация звонка</span><span class="sxs-lookup"><span data-stu-id="a8ce0-152">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="a8ce0-153">Уведомления - входящие</span><span class="sxs-lookup"><span data-stu-id="a8ce0-153">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="a8ce0-154">Запросить</span><span class="sxs-lookup"><span data-stu-id="a8ce0-154">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="a8ce0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8ce0-155">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="a8ce0-156">Уведомления — перенаправление</span><span class="sxs-lookup"><span data-stu-id="a8ce0-156">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="a8ce0-157">Уведомления - завершен</span><span class="sxs-lookup"><span data-stu-id="a8ce0-157">Notification - terminated</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-redirect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
