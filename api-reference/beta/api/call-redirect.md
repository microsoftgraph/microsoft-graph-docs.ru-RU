---
title: 'вызов: redirect'
description: Перенаправление входящего вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 31a2f59c500fb9de53a8b1ed8f274a96cc0c82d4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438617"
---
# <a name="call-redirect"></a><span data-ttu-id="caabf-103">вызов: redirect</span><span class="sxs-lookup"><span data-stu-id="caabf-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caabf-104">Перенаправление входящего вызова.</span><span class="sxs-lookup"><span data-stu-id="caabf-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="caabf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="caabf-105">Permissions</span></span>
<span data-ttu-id="caabf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caabf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="caabf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caabf-108">Permission type</span></span> | <span data-ttu-id="caabf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="caabf-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="caabf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caabf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="caabf-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="caabf-111">Not Supported</span></span>                |
| <span data-ttu-id="caabf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caabf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caabf-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="caabf-113">Not Supported</span></span>                |
| <span data-ttu-id="caabf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="caabf-114">Application</span></span>     | <span data-ttu-id="caabf-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="caabf-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="caabf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caabf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="caabf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caabf-117">Request headers</span></span>
| <span data-ttu-id="caabf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="caabf-118">Name</span></span>          | <span data-ttu-id="caabf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="caabf-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="caabf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="caabf-120">Authorization</span></span> | <span data-ttu-id="caabf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caabf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="caabf-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="caabf-123">Request body</span></span>
<span data-ttu-id="caabf-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="caabf-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="caabf-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="caabf-125">Parameter</span></span>      | <span data-ttu-id="caabf-126">Тип</span><span class="sxs-lookup"><span data-stu-id="caabf-126">Type</span></span>    |<span data-ttu-id="caabf-127">Описание</span><span class="sxs-lookup"><span data-stu-id="caabf-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="caabf-128">targets</span><span class="sxs-lookup"><span data-stu-id="caabf-128">targets</span></span>|<span data-ttu-id="caabf-129">Коллекция [инвитатионпартиЦипантинфо](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="caabf-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="caabf-130">Целевые участники операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="caabf-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="caabf-131">Таржетдиспоситион</span><span class="sxs-lookup"><span data-stu-id="caabf-131">targetDisposition</span></span>|<span data-ttu-id="caabf-132">String</span><span class="sxs-lookup"><span data-stu-id="caabf-132">String</span></span>|<span data-ttu-id="caabf-133">Возможные значения:`default`</span><span class="sxs-lookup"><span data-stu-id="caabf-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="caabf-134">timeout</span><span class="sxs-lookup"><span data-stu-id="caabf-134">timeout</span></span>|<span data-ttu-id="caabf-135">Int32</span><span class="sxs-lookup"><span data-stu-id="caabf-135">Int32</span></span>|<span data-ttu-id="caabf-136">Время ожидания в секундах для операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="caabf-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="caabf-137">Масккалли</span><span class="sxs-lookup"><span data-stu-id="caabf-137">maskCallee</span></span>|<span data-ttu-id="caabf-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="caabf-138">Boolean</span></span>|<span data-ttu-id="caabf-139">Указывает, следует ли маскировать вызываемого вызываемого абонента.</span><span class="sxs-lookup"><span data-stu-id="caabf-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="caabf-140">Масккаллер</span><span class="sxs-lookup"><span data-stu-id="caabf-140">maskCaller</span></span>|<span data-ttu-id="caabf-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="caabf-141">Boolean</span></span>|<span data-ttu-id="caabf-142">Указывает, следует ли маскировать вызывающий абонент.</span><span class="sxs-lookup"><span data-stu-id="caabf-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="caabf-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="caabf-143">Response</span></span>
<span data-ttu-id="caabf-144">Возвращает `202 Accepted` код отклика</span><span class="sxs-lookup"><span data-stu-id="caabf-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="caabf-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="caabf-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="caabf-146">Перенаправление вызова</span><span class="sxs-lookup"><span data-stu-id="caabf-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="caabf-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="caabf-147">Request</span></span>
<span data-ttu-id="caabf-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caabf-148">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="caabf-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="caabf-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="caabf-150">C#</span><span class="sxs-lookup"><span data-stu-id="caabf-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="caabf-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="caabf-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="caabf-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="caabf-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="caabf-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="caabf-153">Response</span></span>

> <span data-ttu-id="caabf-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="caabf-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="caabf-156">Переадресация звонка</span><span class="sxs-lookup"><span data-stu-id="caabf-156">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="caabf-157">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="caabf-157">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="caabf-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="caabf-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="caabf-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="caabf-159">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="caabf-160">Перенаправление уведомлений</span><span class="sxs-lookup"><span data-stu-id="caabf-160">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="caabf-161">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="caabf-161">Notification - terminated</span></span>

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
  ]
}
-->
