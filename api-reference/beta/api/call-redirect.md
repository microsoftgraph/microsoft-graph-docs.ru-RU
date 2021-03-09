---
title: 'вызов: перенаправление'
description: Перенаправление входящего вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fb2aa01474a5c5d29ed1c87978c2d2aacae9ac92
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574897"
---
# <a name="call-redirect"></a><span data-ttu-id="8b896-103">вызов: перенаправление</span><span class="sxs-lookup"><span data-stu-id="8b896-103">call: redirect</span></span>

<span data-ttu-id="8b896-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b896-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b896-105">Перенаправьте входящий вызов, на который еще не ответили [и](./call-answer.md) [не ответили.](./call-reject.md)</span><span class="sxs-lookup"><span data-stu-id="8b896-105">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="8b896-106">Термины "перенаправление" и "переадресовка" вызова используются взаимозаменяемо.</span><span class="sxs-lookup"><span data-stu-id="8b896-106">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="8b896-107">Ожидается, что бот перенаправляет вызов до времени вызова. Текущее значение времени времени — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="8b896-107">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b896-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b896-108">Permissions</span></span>

<span data-ttu-id="8b896-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b896-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b896-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b896-111">Permission type</span></span> | <span data-ttu-id="8b896-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b896-112">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="8b896-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b896-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b896-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b896-114">Not Supported</span></span>                |
| <span data-ttu-id="8b896-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b896-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b896-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b896-116">Not Supported</span></span>                |
| <span data-ttu-id="8b896-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b896-117">Application</span></span>     | <span data-ttu-id="8b896-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="8b896-118">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="8b896-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b896-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /app/calls/{id}/redirect
POST /communications/calls/{id}/redirect
```
> <span data-ttu-id="8b896-120">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="8b896-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="8b896-121">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="8b896-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b896-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b896-122">Request headers</span></span>

| <span data-ttu-id="8b896-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8b896-123">Name</span></span>          | <span data-ttu-id="8b896-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8b896-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8b896-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b896-125">Authorization</span></span> | <span data-ttu-id="8b896-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b896-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b896-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b896-128">Request body</span></span>

<span data-ttu-id="8b896-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8b896-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b896-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="8b896-130">Parameter</span></span>      | <span data-ttu-id="8b896-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b896-131">Type</span></span>    |<span data-ttu-id="8b896-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b896-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b896-133">targets</span><span class="sxs-lookup"><span data-stu-id="8b896-133">targets</span></span>|<span data-ttu-id="8b896-134">Коллекция [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="8b896-134">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="8b896-135">Целевые участники операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="8b896-135">The target participants of the redirect operation.</span></span> <span data-ttu-id="8b896-136">Если задано несколько целевых объектов, это симуляцный вызов.</span><span class="sxs-lookup"><span data-stu-id="8b896-136">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="8b896-137">Это означает, что все целевые объекты будут одновременно звонили и подключена только первая цель, подбираемая.</span><span class="sxs-lookup"><span data-stu-id="8b896-137">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="8b896-138">Мы поддерживаем до 25 целей для simulring.</span><span class="sxs-lookup"><span data-stu-id="8b896-138">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="8b896-139">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="8b896-139">targetDisposition</span></span>|<span data-ttu-id="8b896-140">String</span><span class="sxs-lookup"><span data-stu-id="8b896-140">String</span></span>|<span data-ttu-id="8b896-141">(Неуловимый) Возможные значения: `default` , `simultaneousRing` , `forward` .</span><span class="sxs-lookup"><span data-stu-id="8b896-141">(Deprecated) The possible values are: `default` , `simultaneousRing` , `forward`.</span></span> <span data-ttu-id="8b896-142">Этот параметр обесценен, мы автоматически определяем, является ли это вызовом или симулируется из числа предоставляемых целей.</span><span class="sxs-lookup"><span data-stu-id="8b896-142">This parameter is deprecated, we will automatically identify whether it's a forward call or simulring call from the number of targets provided.</span></span>|
|<span data-ttu-id="8b896-143">timeout</span><span class="sxs-lookup"><span data-stu-id="8b896-143">timeout</span></span>|<span data-ttu-id="8b896-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8b896-144">Int32</span></span>|<span data-ttu-id="8b896-145">Период времени (в секундах) для операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="8b896-145">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="8b896-146">Диапазон значения времени от 15 до 90 секунд включительно.</span><span class="sxs-lookup"><span data-stu-id="8b896-146">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="8b896-147">Значение времени по умолчанию — 55 секунд для одной цели и 60 секунд для нескольких целей (при условии изменения).</span><span class="sxs-lookup"><span data-stu-id="8b896-147">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="8b896-148">maskCallee</span><span class="sxs-lookup"><span data-stu-id="8b896-148">maskCallee</span></span>|<span data-ttu-id="8b896-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b896-149">Boolean</span></span>|<span data-ttu-id="8b896-150">Указывает, следует ли скрывать вызываемую от вызываемой.</span><span class="sxs-lookup"><span data-stu-id="8b896-150">Indicates whether the callee is to be hidden from the caller.</span></span> <span data-ttu-id="8b896-151">Если это так, то идентификатор вызывающего пользователя — это идентификатор бота.</span><span class="sxs-lookup"><span data-stu-id="8b896-151">If true, then the callee identity is the bot identity.</span></span> <span data-ttu-id="8b896-152">По умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="8b896-152">Default: false.</span></span>|
|<span data-ttu-id="8b896-153">maskCaller</span><span class="sxs-lookup"><span data-stu-id="8b896-153">maskCaller</span></span>|<span data-ttu-id="8b896-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b896-154">Boolean</span></span>|<span data-ttu-id="8b896-155">Указывает, следует ли скрывать вызываемую от вызываемой стороны.</span><span class="sxs-lookup"><span data-stu-id="8b896-155">Indicates whether the caller is to be hidden from the callee.</span></span> <span data-ttu-id="8b896-156">Если это так, то идентификатор вызывающего пользователя — это идентификатор бота.</span><span class="sxs-lookup"><span data-stu-id="8b896-156">If true, then the caller identity is the bot identity.</span></span> <span data-ttu-id="8b896-157">По умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="8b896-157">Default: false.</span></span>|
|<span data-ttu-id="8b896-158">callbackUri</span><span class="sxs-lookup"><span data-stu-id="8b896-158">callbackUri</span></span>|<span data-ttu-id="8b896-159">String</span><span class="sxs-lookup"><span data-stu-id="8b896-159">String</span></span>|<span data-ttu-id="8b896-160">Это позволяет ботам предоставлять определенный URI вызова для текущего вызова для получения более поздних уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8b896-160">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="8b896-161">Если это свойство не установлено, вместо него будет использоваться глобальный URI вызова бота.</span><span class="sxs-lookup"><span data-stu-id="8b896-161">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="8b896-162">Это должно быть `https` .</span><span class="sxs-lookup"><span data-stu-id="8b896-162">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="8b896-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b896-163">Response</span></span>
<span data-ttu-id="8b896-164">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="8b896-164">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8b896-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b896-165">Examples</span></span>
<span data-ttu-id="8b896-166">В этих примерах будет освещаться рабочий процесс уведомления о входящих вызовах и его перенаправление.</span><span class="sxs-lookup"><span data-stu-id="8b896-166">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="8b896-167">**Примечание:** Объекты ответа, показанные здесь, могут быть сокращены для читаемости.</span><span class="sxs-lookup"><span data-stu-id="8b896-167">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="8b896-168">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b896-168">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="8b896-169">Пример 1. Переадвока вызова в целевой адрес</span><span class="sxs-lookup"><span data-stu-id="8b896-169">Example 1: Forward a call to a target</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="8b896-170">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="8b896-170">Notification - incoming</span></span>
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

#### <a name="request"></a><span data-ttu-id="8b896-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b896-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b896-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b896-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request", 
  "name": "call-redirect"
} -->
``` http
POST https://graph.microsoft.com/beta/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect
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
# <a name="c"></a>[<span data-ttu-id="8b896-173">C#</span><span class="sxs-lookup"><span data-stu-id="8b896-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b896-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b896-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b896-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b896-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b896-176">Java</span><span class="sxs-lookup"><span data-stu-id="8b896-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8b896-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b896-177">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="notification---terminated"></a><span data-ttu-id="8b896-178">Уведомление — прекращено</span><span class="sxs-lookup"><span data-stu-id="8b896-178">Notification - terminated</span></span>

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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="8b896-179">Пример 2. Перенацелив вызов на несколько целей с одновременным кольцом</span><span class="sxs-lookup"><span data-stu-id="8b896-179">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="8b896-180">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="8b896-180">Notification - incoming</span></span>

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
              "id": "ec040873-8235-45fd-a403-c7259a5a548e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
      }
    }
  ]
}
```

#### <a name="request"></a><span data-ttu-id="8b896-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b896-181">Request</span></span>

<!-- {
  "blockType": "ignored", 
  "name": "call-redirect-simuring"
} -->

``` http
POST https://graph.microsoft.com/beta/communications/calls/481f0b00-ffff-4ca1-8c67-a5f1e31e8e82/redirect
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

#### <a name="response"></a><span data-ttu-id="8b896-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b896-182">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

#### <a name="notification---terminated"></a><span data-ttu-id="8b896-183">Уведомление — прекращено</span><span class="sxs-lookup"><span data-stu-id="8b896-183">Notification - terminated</span></span>

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
              "id": "ec040873-8235-45fd-a403-c7259a5a548e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
      }
    }
  ]
}
```

### <a name="example-3-forward-a-call-to-a-pstn-number"></a><span data-ttu-id="8b896-184">Пример 3. Переадмить вызов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="8b896-184">Example 3: Forward a call to a PSTN number</span></span>

<span data-ttu-id="8b896-185">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="8b896-185">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="8b896-186">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="8b896-186">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="8b896-187">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="8b896-187">Notification - incoming</span></span>
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

#### <a name="request"></a><span data-ttu-id="8b896-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b896-188">Request</span></span>

<!-- {
  "blockType": "request", 
  "name": "call-redirect"
} -->
``` http
POST https://graph.microsoft.com/beta/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect
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
#### <a name="response"></a><span data-ttu-id="8b896-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b896-189">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="notification---terminated"></a><span data-ttu-id="8b896-190">Уведомление — прекращено</span><span class="sxs-lookup"><span data-stu-id="8b896-190">Notification - terminated</span></span>

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


