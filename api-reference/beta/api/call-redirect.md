---
title: 'вызов: redirect'
description: Перенаправление входящего вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8291751b4dfc74fcd2f4ccfd194cc8bfbe66c482
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636326"
---
# <a name="call-redirect"></a><span data-ttu-id="c49b1-103">вызов: redirect</span><span class="sxs-lookup"><span data-stu-id="c49b1-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c49b1-104">Перенаправление входящего вызова.</span><span class="sxs-lookup"><span data-stu-id="c49b1-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c49b1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c49b1-105">Permissions</span></span>
<span data-ttu-id="c49b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c49b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c49b1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c49b1-108">Permission type</span></span> | <span data-ttu-id="c49b1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c49b1-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="c49b1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c49b1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c49b1-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c49b1-111">Not Supported</span></span>                |
| <span data-ttu-id="c49b1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c49b1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c49b1-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c49b1-113">Not Supported</span></span>                |
| <span data-ttu-id="c49b1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c49b1-114">Application</span></span>     | <span data-ttu-id="c49b1-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="c49b1-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="c49b1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c49b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="c49b1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c49b1-117">Request headers</span></span>
| <span data-ttu-id="c49b1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c49b1-118">Name</span></span>          | <span data-ttu-id="c49b1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c49b1-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c49b1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c49b1-120">Authorization</span></span> | <span data-ttu-id="c49b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c49b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c49b1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c49b1-123">Request body</span></span>
<span data-ttu-id="c49b1-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c49b1-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c49b1-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="c49b1-125">Parameter</span></span>      | <span data-ttu-id="c49b1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c49b1-126">Type</span></span>    |<span data-ttu-id="c49b1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c49b1-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c49b1-128">targets</span><span class="sxs-lookup"><span data-stu-id="c49b1-128">targets</span></span>|<span data-ttu-id="c49b1-129">Коллекция [инвитатионпартиЦипантинфо](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="c49b1-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="c49b1-130">Целевые участники операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="c49b1-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="c49b1-131">Таржетдиспоситион</span><span class="sxs-lookup"><span data-stu-id="c49b1-131">targetDisposition</span></span>|<span data-ttu-id="c49b1-132">String</span><span class="sxs-lookup"><span data-stu-id="c49b1-132">String</span></span>|<span data-ttu-id="c49b1-133">Возможные значения:`default`</span><span class="sxs-lookup"><span data-stu-id="c49b1-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="c49b1-134">timeout</span><span class="sxs-lookup"><span data-stu-id="c49b1-134">timeout</span></span>|<span data-ttu-id="c49b1-135">Int32</span><span class="sxs-lookup"><span data-stu-id="c49b1-135">Int32</span></span>|<span data-ttu-id="c49b1-136">Время ожидания в секундах для операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="c49b1-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="c49b1-137">Масккалли</span><span class="sxs-lookup"><span data-stu-id="c49b1-137">maskCallee</span></span>|<span data-ttu-id="c49b1-138">Логический</span><span class="sxs-lookup"><span data-stu-id="c49b1-138">Boolean</span></span>|<span data-ttu-id="c49b1-139">Указывает, следует ли маскировать вызываемого вызываемого абонента.</span><span class="sxs-lookup"><span data-stu-id="c49b1-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="c49b1-140">Масккаллер</span><span class="sxs-lookup"><span data-stu-id="c49b1-140">maskCaller</span></span>|<span data-ttu-id="c49b1-141">Логический</span><span class="sxs-lookup"><span data-stu-id="c49b1-141">Boolean</span></span>|<span data-ttu-id="c49b1-142">Указывает, следует ли маскировать вызывающий абонент.</span><span class="sxs-lookup"><span data-stu-id="c49b1-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="c49b1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c49b1-143">Response</span></span>
<span data-ttu-id="c49b1-144">Возвращает `202 Accepted` код отклика</span><span class="sxs-lookup"><span data-stu-id="c49b1-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="c49b1-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="c49b1-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="c49b1-146">Перенаправление вызова</span><span class="sxs-lookup"><span data-stu-id="c49b1-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="c49b1-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c49b1-147">Request</span></span>
<span data-ttu-id="c49b1-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c49b1-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c49b1-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c49b1-149">Response</span></span>

> <span data-ttu-id="c49b1-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c49b1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c49b1-152">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="c49b1-152">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c49b1-153">Язык</span><span class="sxs-lookup"><span data-stu-id="c49b1-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-redirect-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="forward-a-call"></a><span data-ttu-id="c49b1-154">Переадресация звонка</span><span class="sxs-lookup"><span data-stu-id="c49b1-154">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="c49b1-155">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="c49b1-155">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="c49b1-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="c49b1-156">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="c49b1-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c49b1-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="c49b1-158">Перенаправление уведомлений</span><span class="sxs-lookup"><span data-stu-id="c49b1-158">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="c49b1-159">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="c49b1-159">Notification - terminated</span></span>

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
    "Error: /api-reference/beta/api/call-redirect.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
