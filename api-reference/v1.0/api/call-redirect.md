---
title: 'вызов: перенаправление'
description: Перенаправление входящего вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5f121c5cc6a3422b7945dfb5c249ae72a706a548
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665548"
---
# <a name="call-redirect"></a><span data-ttu-id="6b5c8-103">вызов: перенаправление</span><span class="sxs-lookup"><span data-stu-id="6b5c8-103">call: redirect</span></span>

<span data-ttu-id="6b5c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b5c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b5c8-105">Перенаправьте входящий вызов, на который еще не ответили [и](./call-answer.md) [не ответили.](./call-reject.md)</span><span class="sxs-lookup"><span data-stu-id="6b5c8-105">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="6b5c8-106">Термины "перенаправление" и "переадресовка" вызова используются взаимозаменяемо.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-106">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="6b5c8-107">Ожидается, что бот перенаправляет вызов до времени вызова. Текущее значение времени времени — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-107">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b5c8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b5c8-108">Permissions</span></span>

<span data-ttu-id="6b5c8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b5c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b5c8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b5c8-111">Permission type</span></span> | <span data-ttu-id="6b5c8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b5c8-112">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="6b5c8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b5c8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b5c8-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6b5c8-114">Not Supported</span></span>                |
| <span data-ttu-id="6b5c8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b5c8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b5c8-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6b5c8-116">Not Supported</span></span>                |
| <span data-ttu-id="6b5c8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6b5c8-117">Application</span></span>     | <span data-ttu-id="6b5c8-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="6b5c8-118">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="6b5c8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b5c8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="6b5c8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b5c8-120">Request headers</span></span>

| <span data-ttu-id="6b5c8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6b5c8-121">Name</span></span>          | <span data-ttu-id="6b5c8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6b5c8-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6b5c8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b5c8-123">Authorization</span></span> | <span data-ttu-id="6b5c8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b5c8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b5c8-126">Request body</span></span>

<span data-ttu-id="6b5c8-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6b5c8-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="6b5c8-128">Parameter</span></span>      | <span data-ttu-id="6b5c8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6b5c8-129">Type</span></span>    |<span data-ttu-id="6b5c8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6b5c8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b5c8-131">targets</span><span class="sxs-lookup"><span data-stu-id="6b5c8-131">targets</span></span>|<span data-ttu-id="6b5c8-132">Коллекция [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="6b5c8-132">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="6b5c8-133">Целевые участники операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-133">The target participants of the redirect operation.</span></span> <span data-ttu-id="6b5c8-134">Если задано несколько целевых объектов, это симуляцный вызов.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-134">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="6b5c8-135">Это означает, что все целевые объекты будут одновременно звонили и подключена только первая цель, подбираемая.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-135">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="6b5c8-136">Мы поддерживаем до 25 целей для simulring.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-136">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="6b5c8-137">timeout</span><span class="sxs-lookup"><span data-stu-id="6b5c8-137">timeout</span></span>|<span data-ttu-id="6b5c8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="6b5c8-138">Int32</span></span>|<span data-ttu-id="6b5c8-139">Период времени (в секундах) для операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-139">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="6b5c8-140">Диапазон значения времени от 15 до 90 секунд включительно.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-140">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="6b5c8-141">Значение времени по умолчанию — 55 секунд для одной цели и 60 секунд для нескольких целей (при условии изменения).</span><span class="sxs-lookup"><span data-stu-id="6b5c8-141">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="6b5c8-142">callbackUri</span><span class="sxs-lookup"><span data-stu-id="6b5c8-142">callbackUri</span></span>|<span data-ttu-id="6b5c8-143">String</span><span class="sxs-lookup"><span data-stu-id="6b5c8-143">String</span></span>|<span data-ttu-id="6b5c8-144">Это позволяет ботам предоставлять определенный URI вызова для текущего вызова для получения более поздних уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-144">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="6b5c8-145">Если это свойство не установлено, вместо него будет использоваться глобальный URI вызова бота.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-145">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="6b5c8-146">Это должно быть `https` .</span><span class="sxs-lookup"><span data-stu-id="6b5c8-146">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="6b5c8-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b5c8-147">Response</span></span>
<span data-ttu-id="6b5c8-148">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-148">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6b5c8-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b5c8-149">Examples</span></span>
<span data-ttu-id="6b5c8-150">В этих примерах будет освещаться рабочий процесс уведомления о входящих вызовах и его перенаправление.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-150">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="6b5c8-151">**Примечание:** Объекты ответа, показанные здесь, могут быть сокращены для читаемости.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-151">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="6b5c8-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-152">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="6b5c8-153">Пример 1. Переадвока вызова в целевой объект</span><span class="sxs-lookup"><span data-stu-id="6b5c8-153">Example 1: Forward a Call to a Target</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6b5c8-154">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6b5c8-154">Notification - incoming</span></span>
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

##### <a name="request"></a><span data-ttu-id="6b5c8-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b5c8-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6b5c8-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b5c8-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request", 
  "name": "call-redirect-1"
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
# <a name="c"></a>[<span data-ttu-id="6b5c8-157">C#</span><span class="sxs-lookup"><span data-stu-id="6b5c8-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b5c8-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b5c8-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b5c8-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b5c8-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b5c8-160">Java</span><span class="sxs-lookup"><span data-stu-id="6b5c8-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b5c8-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b5c8-161">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---terminated"></a><span data-ttu-id="6b5c8-162">Уведомление — прекращено</span><span class="sxs-lookup"><span data-stu-id="6b5c8-162">Notification - terminated</span></span>

<!-- {
  "blockType": "example", 
  "name": "call-redirect-2"
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

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="6b5c8-163">Пример 2. Перенацелив вызов на несколько целей с одновременным кольцом</span><span class="sxs-lookup"><span data-stu-id="6b5c8-163">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6b5c8-164">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6b5c8-164">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="6b5c8-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b5c8-165">Request</span></span>

<!-- {
  "blockType": "ignored", 
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

##### <a name="response"></a><span data-ttu-id="6b5c8-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b5c8-166">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

##### <a name="notification---terminated"></a><span data-ttu-id="6b5c8-167">Уведомление — прекращено</span><span class="sxs-lookup"><span data-stu-id="6b5c8-167">Notification - terminated</span></span>

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

### <a name="example-3-forward-a-call-to-a-pstn-number"></a><span data-ttu-id="6b5c8-168">Пример 3. Переадмить вызов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="6b5c8-168">Example 3: Forward a call to a PSTN number</span></span>

<span data-ttu-id="6b5c8-169">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-169">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="6b5c8-170">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="6b5c8-170">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="6b5c8-171">**Примечание.** Телефон ID — это номер телефона в формате E.164.</span><span class="sxs-lookup"><span data-stu-id="6b5c8-171">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="6b5c8-172">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6b5c8-172">Notification - incoming</span></span>
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
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "applicationInstance": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "PstnAppInstance",
                "id": "7629bdce-046c-4903-86b4-a8f718277e1a",
                "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
              }
            },
            "endpointType": "default",
            "id": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
            "region": "amer",
            "languageId": null
          }
        ],
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

#### <a name="request"></a><span data-ttu-id="6b5c8-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b5c8-173">Request</span></span>

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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}
```
#### <a name="response"></a><span data-ttu-id="6b5c8-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b5c8-174">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="notification---terminated"></a><span data-ttu-id="6b5c8-175">Уведомление — прекращено</span><span class="sxs-lookup"><span data-stu-id="6b5c8-175">Notification - terminated</span></span>

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
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "applicationInstance": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "PstnAppInstance",
                "id": "7629bdce-046c-4903-86b4-a8f718277e1a",
                "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
              }
            },
            "endpointType": "default",
            "id": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
            "region": "amer",
            "languageId": null
          }
        ],
        "answeredBy": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "encrypted": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "1xt4uextl99sdzwdxuvdxrvgrv8gehcq7jdgf9yhzeto"
            }
          },
          "endpointType": "default"
        },
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
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

