---
title: 'вызов: redirect'
description: Перенаправление входящего вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 166218acee43d69495f68721445678235c1e62f8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518681"
---
# <a name="call-redirect"></a><span data-ttu-id="5a853-103">вызов: redirect</span><span class="sxs-lookup"><span data-stu-id="5a853-103">call: redirect</span></span>

<span data-ttu-id="5a853-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a853-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a853-105">Перенаправление входящего звонка, который еще не [отвечал](./call-answer.md) или не был [отклонен](./call-reject.md) .</span><span class="sxs-lookup"><span data-stu-id="5a853-105">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="5a853-106">Термины "перенаправление" и "переадресация" используются взаимозаменяемыми.</span><span class="sxs-lookup"><span data-stu-id="5a853-106">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="5a853-107">Ожидается, что Bot перенаправляет вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="5a853-107">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a853-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a853-108">Permissions</span></span>

<span data-ttu-id="5a853-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a853-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a853-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a853-111">Permission type</span></span> | <span data-ttu-id="5a853-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a853-112">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="5a853-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a853-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a853-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5a853-114">Not Supported</span></span>                |
| <span data-ttu-id="5a853-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a853-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a853-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5a853-116">Not Supported</span></span>                |
| <span data-ttu-id="5a853-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a853-117">Application</span></span>     | <span data-ttu-id="5a853-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="5a853-118">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="5a853-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a853-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="5a853-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a853-120">Request headers</span></span>

| <span data-ttu-id="5a853-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5a853-121">Name</span></span>          | <span data-ttu-id="5a853-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5a853-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5a853-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a853-123">Authorization</span></span> | <span data-ttu-id="5a853-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a853-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a853-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a853-126">Request body</span></span>

<span data-ttu-id="5a853-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5a853-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a853-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="5a853-128">Parameter</span></span>      | <span data-ttu-id="5a853-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5a853-129">Type</span></span>    |<span data-ttu-id="5a853-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5a853-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a853-131">targets</span><span class="sxs-lookup"><span data-stu-id="5a853-131">targets</span></span>|<span data-ttu-id="5a853-132">Коллекция [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="5a853-132">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="5a853-133">Целевые участники операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="5a853-133">The target participants of the redirect operation.</span></span> <span data-ttu-id="5a853-134">Если указано несколько целевых объектов, вызывается выполнение.</span><span class="sxs-lookup"><span data-stu-id="5a853-134">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="5a853-135">Это означает, что все целевые объекты будут находиться в одном и том же периоде, и будет подключен только первый целевой объект.</span><span class="sxs-lookup"><span data-stu-id="5a853-135">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="5a853-136">Поддерживается до 25 целевых объектов для выполнение.</span><span class="sxs-lookup"><span data-stu-id="5a853-136">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="5a853-137">timeout</span><span class="sxs-lookup"><span data-stu-id="5a853-137">timeout</span></span>|<span data-ttu-id="5a853-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5a853-138">Int32</span></span>|<span data-ttu-id="5a853-139">Время ожидания (в секундах) для операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="5a853-139">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="5a853-140">Диапазон значений времени ожидания составляет от 15 до 90 секунд включительно.</span><span class="sxs-lookup"><span data-stu-id="5a853-140">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="5a853-141">Значение времени ожидания по умолчанию составляет 55 секунд для одной цели и 60 секунд для нескольких целевых объектов (подлежит изменению).</span><span class="sxs-lookup"><span data-stu-id="5a853-141">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="5a853-142">callbackUri</span><span class="sxs-lookup"><span data-stu-id="5a853-142">callbackUri</span></span>|<span data-ttu-id="5a853-143">String</span><span class="sxs-lookup"><span data-stu-id="5a853-143">String</span></span>|<span data-ttu-id="5a853-144">Это позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления позже.</span><span class="sxs-lookup"><span data-stu-id="5a853-144">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="5a853-145">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="5a853-145">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="5a853-146">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="5a853-146">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="5a853-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a853-147">Response</span></span>
<span data-ttu-id="5a853-148">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="5a853-148">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5a853-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="5a853-149">Examples</span></span>
<span data-ttu-id="5a853-150">В этих примерах рассматривается рабочий процесс уведомления о входящем вызове и способ перенаправления этого вызова.</span><span class="sxs-lookup"><span data-stu-id="5a853-150">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="5a853-151">**Примечание:** Показанные здесь объекты отклика могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5a853-151">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="5a853-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a853-152">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="5a853-153">Пример 1: Переадресация вызова на целевой объект</span><span class="sxs-lookup"><span data-stu-id="5a853-153">Example 1: Forward a Call to a Target</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="5a853-154">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="5a853-154">Notification - incoming</span></span>
<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "incoming",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="5a853-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a853-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5a853-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a853-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request", 
  "name": "call-redirect"
} -->
``` http
POST https://graph.microsoft.com/v1.0/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect
Content-Type: application/json

{
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "application": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "test bot 2",
          "id": "22bfd41f-550e-477d-8789-f6f7bd2a5e8b"
        }
      }
    }
  ],
  "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}
```
# <a name="c"></a>[<span data-ttu-id="5a853-157">C#</span><span class="sxs-lookup"><span data-stu-id="5a853-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a853-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a853-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a853-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a853-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a853-160">Java</span><span class="sxs-lookup"><span data-stu-id="5a853-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5a853-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a853-161">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---terminated"></a><span data-ttu-id="5a853-162">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="5a853-162">Notification - terminated</span></span>

<!-- {
  "blockType": "example", 
  "name": "call-redirect"
} -->
``` http
POST https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039
Content-Type: application/json
```

<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
} -->
``` json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="5a853-163">Пример 2: Переадресация вызова на несколько целевых объектов с одновременным кольцом</span><span class="sxs-lookup"><span data-stu-id="5a853-163">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="5a853-164">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="5a853-164">Notification - incoming</span></span>

<!-- {
  "blockType": "example", 
  "name": "call-redirect"
} -->
``` http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/481f0b00-ffff-4ca1-8c67-a5f1e31e8e82",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "incoming",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "ec040873-8235-45fd-a403-c7259a5a548e"
            }
          },
          "region": "amer"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="5a853-165">Запросить</span><span class="sxs-lookup"><span data-stu-id="5a853-165">Request</span></span>

<!-- {
  "blockType": "request", 
  "name": "call-redirect-simuring"
} -->

``` http
POST https://graph.microsoft.com/v1.0/communications/calls/481f0b00-ffff-4ca1-8c67-a5f1e31e8e82/redirect
Content-Type: application/json

{
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "test user",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b1253"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "test user 2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c9c3f3"
        }
      }
    }
  ],
  "routingPolicies": [
    "disableForwarding"
  ],
  "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}
```

##### <a name="response"></a><span data-ttu-id="5a853-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a853-166">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

##### <a name="notification---terminated"></a><span data-ttu-id="5a853-167">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="5a853-167">Notification - terminated</span></span>

<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
} -->

``` http
POST https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "ec040873-8235-45fd-a403-c7259a5a548e"
            }
          },
          "region": "amer"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
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
