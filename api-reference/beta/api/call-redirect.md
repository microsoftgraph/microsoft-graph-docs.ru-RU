---
title: 'вызов: redirect'
description: Перенаправление входящего вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 51db3a87dbbfae18bb3b1651d34dc9cf1ca28725
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636696"
---
# <a name="call-redirect"></a><span data-ttu-id="6b321-103">вызов: redirect</span><span class="sxs-lookup"><span data-stu-id="6b321-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b321-104">Перенаправление входящего звонка, который еще не [отвечал](./call-answer.md) или не был [отклонен](./call-reject.md) .</span><span class="sxs-lookup"><span data-stu-id="6b321-104">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="6b321-105">Термины "перенаправление" и "переадресация" используются взаимозаменяемыми.</span><span class="sxs-lookup"><span data-stu-id="6b321-105">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="6b321-106">Ожидается, что Bot перенаправляет вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="6b321-106">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b321-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b321-107">Permissions</span></span>

<span data-ttu-id="6b321-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b321-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b321-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b321-110">Permission type</span></span> | <span data-ttu-id="6b321-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b321-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="6b321-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b321-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b321-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6b321-113">Not Supported</span></span>                |
| <span data-ttu-id="6b321-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b321-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b321-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6b321-115">Not Supported</span></span>                |
| <span data-ttu-id="6b321-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6b321-116">Application</span></span>     | <span data-ttu-id="6b321-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="6b321-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="6b321-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b321-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /app/calls/{id}/redirect
POST /communications/calls/{id}/redirect
```
> <span data-ttu-id="6b321-119">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="6b321-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="6b321-120">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="6b321-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b321-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b321-121">Request headers</span></span>

| <span data-ttu-id="6b321-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6b321-122">Name</span></span>          | <span data-ttu-id="6b321-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6b321-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6b321-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b321-124">Authorization</span></span> | <span data-ttu-id="6b321-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b321-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b321-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b321-127">Request body</span></span>

<span data-ttu-id="6b321-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6b321-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6b321-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="6b321-129">Parameter</span></span>      | <span data-ttu-id="6b321-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6b321-130">Type</span></span>    |<span data-ttu-id="6b321-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6b321-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b321-132">targets</span><span class="sxs-lookup"><span data-stu-id="6b321-132">targets</span></span>|<span data-ttu-id="6b321-133">Коллекция [инвитатионпартиЦипантинфо](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="6b321-133">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="6b321-134">Целевые участники операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="6b321-134">The target participants of the redirect operation.</span></span> <span data-ttu-id="6b321-135">Если указано несколько целевых объектов, вызывается выполнение.</span><span class="sxs-lookup"><span data-stu-id="6b321-135">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="6b321-136">Это означает, что все целевые объекты будут находиться в одном и том же периоде, и будет подключен только первый целевой объект.</span><span class="sxs-lookup"><span data-stu-id="6b321-136">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="6b321-137">Поддерживается до 25 целевых объектов для выполнение.</span><span class="sxs-lookup"><span data-stu-id="6b321-137">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="6b321-138">таржетдиспоситион</span><span class="sxs-lookup"><span data-stu-id="6b321-138">targetDisposition</span></span>|<span data-ttu-id="6b321-139">String</span><span class="sxs-lookup"><span data-stu-id="6b321-139">String</span></span>|<span data-ttu-id="6b321-140">Устаревшие Возможные значения: `default` , `simultaneousRing` ,. `forward`</span><span class="sxs-lookup"><span data-stu-id="6b321-140">(Deprecated) The possible values are: `default` , `simultaneousRing` , `forward`.</span></span> <span data-ttu-id="6b321-141">Этот параметр является нерекомендуемым, мы автоматически вычислим, является ли это вызов переадресацией или вызовом выполнение из указанного количества целевых объектов.</span><span class="sxs-lookup"><span data-stu-id="6b321-141">This parameter is deprecated, we will automatically identify whether it's a forward call or simulring call from the number of targets provided.</span></span>|
|<span data-ttu-id="6b321-142">timeout</span><span class="sxs-lookup"><span data-stu-id="6b321-142">timeout</span></span>|<span data-ttu-id="6b321-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6b321-143">Int32</span></span>|<span data-ttu-id="6b321-144">Время ожидания (в секундах) для операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="6b321-144">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="6b321-145">Диапазон значений времени ожидания составляет от 15 до 90 секунд включительно.</span><span class="sxs-lookup"><span data-stu-id="6b321-145">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="6b321-146">Значение времени ожидания по умолчанию составляет 55 секунд для одной цели и 60 секунд для нескольких целевых объектов (подлежит изменению).</span><span class="sxs-lookup"><span data-stu-id="6b321-146">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="6b321-147">масккалли</span><span class="sxs-lookup"><span data-stu-id="6b321-147">maskCallee</span></span>|<span data-ttu-id="6b321-148">Логический</span><span class="sxs-lookup"><span data-stu-id="6b321-148">Boolean</span></span>|<span data-ttu-id="6b321-149">Указывает, следует ли скрыть вызываемого абонента от вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="6b321-149">Indicates whether the callee is to be hidden from the caller.</span></span> <span data-ttu-id="6b321-150">Если этот параметр имеет значение true, идентификатором вызываемого абонента является "bot".</span><span class="sxs-lookup"><span data-stu-id="6b321-150">If true, then the callee identity is the bot identity.</span></span> <span data-ttu-id="6b321-151">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="6b321-151">Default: false.</span></span>|
|<span data-ttu-id="6b321-152">масккаллер</span><span class="sxs-lookup"><span data-stu-id="6b321-152">maskCaller</span></span>|<span data-ttu-id="6b321-153">Логический</span><span class="sxs-lookup"><span data-stu-id="6b321-153">Boolean</span></span>|<span data-ttu-id="6b321-154">Указывает, следует ли скрыть абонента от вызываемого абонента.</span><span class="sxs-lookup"><span data-stu-id="6b321-154">Indicates whether the caller is to be hidden from the callee.</span></span> <span data-ttu-id="6b321-155">Если задано значение true, идентификатором звонящего является идентификатор Bot.</span><span class="sxs-lookup"><span data-stu-id="6b321-155">If true, then the caller identity is the bot identity.</span></span> <span data-ttu-id="6b321-156">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="6b321-156">Default: false.</span></span>|
|<span data-ttu-id="6b321-157">callbackUri</span><span class="sxs-lookup"><span data-stu-id="6b321-157">callbackUri</span></span>|<span data-ttu-id="6b321-158">String</span><span class="sxs-lookup"><span data-stu-id="6b321-158">String</span></span>|<span data-ttu-id="6b321-159">Это позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления позже.</span><span class="sxs-lookup"><span data-stu-id="6b321-159">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="6b321-160">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="6b321-160">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="6b321-161">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="6b321-161">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="6b321-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b321-162">Response</span></span>
<span data-ttu-id="6b321-163">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="6b321-163">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6b321-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b321-164">Examples</span></span>
<span data-ttu-id="6b321-165">В этих примерах рассматривается рабочий процесс уведомления о входящем вызове и способ перенаправления этого вызова.</span><span class="sxs-lookup"><span data-stu-id="6b321-165">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="6b321-166">**Примечание:** Показанные здесь объекты отклика могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b321-166">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="6b321-167">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b321-167">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="6b321-168">Пример 1: Переадресация вызова на целевой объект</span><span class="sxs-lookup"><span data-stu-id="6b321-168">Example 1: Forward a Call to a Target</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6b321-169">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6b321-169">Notification - incoming</span></span>
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

##### <a name="request"></a><span data-ttu-id="6b321-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b321-170">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6b321-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b321-171">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b321-172">C#</span><span class="sxs-lookup"><span data-stu-id="6b321-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b321-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b321-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b321-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b321-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b321-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b321-175">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---terminated"></a><span data-ttu-id="6b321-176">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="6b321-176">Notification - terminated</span></span>

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

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="6b321-177">Пример 2: Переадресация вызова на несколько целевых объектов с одновременным кольцом</span><span class="sxs-lookup"><span data-stu-id="6b321-177">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6b321-178">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6b321-178">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="6b321-179">Запросить</span><span class="sxs-lookup"><span data-stu-id="6b321-179">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="6b321-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b321-180">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

##### <a name="notification---terminated"></a><span data-ttu-id="6b321-181">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="6b321-181">Notification - terminated</span></span>

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
