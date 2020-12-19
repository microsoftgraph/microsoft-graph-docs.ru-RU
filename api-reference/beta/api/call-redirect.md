---
title: 'call: redirect'
description: Перенаправление входящего вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8a3919c2a84b8b248f81599359dcba92d58f830f
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719683"
---
# <a name="call-redirect"></a><span data-ttu-id="6ee99-103">call: redirect</span><span class="sxs-lookup"><span data-stu-id="6ee99-103">call: redirect</span></span>

<span data-ttu-id="6ee99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ee99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ee99-105">Перенаправление входящих вызовов, на которые еще не был ответ [или](./call-answer.md) [отклонен.](./call-reject.md)</span><span class="sxs-lookup"><span data-stu-id="6ee99-105">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="6ee99-106">Термины "перенаправление" и "переадресовка" вызова используются взаимозаменяемо.</span><span class="sxs-lookup"><span data-stu-id="6ee99-106">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="6ee99-107">Ожидается, что бот перенаправит вызов до того, как он по инет. Текущее значение времени простоя составляет 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="6ee99-107">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ee99-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ee99-108">Permissions</span></span>

<span data-ttu-id="6ee99-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ee99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ee99-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ee99-111">Permission type</span></span> | <span data-ttu-id="6ee99-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ee99-112">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="6ee99-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ee99-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ee99-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6ee99-114">Not Supported</span></span>                |
| <span data-ttu-id="6ee99-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ee99-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ee99-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6ee99-116">Not Supported</span></span>                |
| <span data-ttu-id="6ee99-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6ee99-117">Application</span></span>     | <span data-ttu-id="6ee99-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="6ee99-118">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="6ee99-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ee99-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /app/calls/{id}/redirect
POST /communications/calls/{id}/redirect
```
> <span data-ttu-id="6ee99-120">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="6ee99-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="6ee99-121">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="6ee99-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ee99-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ee99-122">Request headers</span></span>

| <span data-ttu-id="6ee99-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6ee99-123">Name</span></span>          | <span data-ttu-id="6ee99-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6ee99-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6ee99-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ee99-125">Authorization</span></span> | <span data-ttu-id="6ee99-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ee99-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ee99-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ee99-128">Request body</span></span>

<span data-ttu-id="6ee99-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6ee99-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6ee99-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="6ee99-130">Parameter</span></span>      | <span data-ttu-id="6ee99-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6ee99-131">Type</span></span>    |<span data-ttu-id="6ee99-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6ee99-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ee99-133">targets</span><span class="sxs-lookup"><span data-stu-id="6ee99-133">targets</span></span>|<span data-ttu-id="6ee99-134">Коллекция [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="6ee99-134">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="6ee99-135">Целевые участники операции перенаправления.</span><span class="sxs-lookup"><span data-stu-id="6ee99-135">The target participants of the redirect operation.</span></span> <span data-ttu-id="6ee99-136">Если указано несколько целевых объектов, это имитирующие вызовы.</span><span class="sxs-lookup"><span data-stu-id="6ee99-136">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="6ee99-137">Это означает, что все целевые объекты будут одновременно рангом, и будет подключен только первый целевой объект, который выбирает.</span><span class="sxs-lookup"><span data-stu-id="6ee99-137">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="6ee99-138">Мы поддерживаем до 25 целевых объектов для моделирования.</span><span class="sxs-lookup"><span data-stu-id="6ee99-138">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="6ee99-139">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="6ee99-139">targetDisposition</span></span>|<span data-ttu-id="6ee99-140">String</span><span class="sxs-lookup"><span data-stu-id="6ee99-140">String</span></span>|<span data-ttu-id="6ee99-141">(Неподготовлено) Возможные значения: `default` , `simultaneousRing` , `forward` .</span><span class="sxs-lookup"><span data-stu-id="6ee99-141">(Deprecated) The possible values are: `default` , `simultaneousRing` , `forward`.</span></span> <span data-ttu-id="6ee99-142">Этот параметр является неподготовленным, мы автоматически определяем, является ли он переадреательным вызовом или имитирует вызов из числа заданных целей.</span><span class="sxs-lookup"><span data-stu-id="6ee99-142">This parameter is deprecated, we will automatically identify whether it's a forward call or simulring call from the number of targets provided.</span></span>|
|<span data-ttu-id="6ee99-143">timeout</span><span class="sxs-lookup"><span data-stu-id="6ee99-143">timeout</span></span>|<span data-ttu-id="6ee99-144">Int32</span><span class="sxs-lookup"><span data-stu-id="6ee99-144">Int32</span></span>|<span data-ttu-id="6ee99-145">Время действия операции перенаправления (в секундах).</span><span class="sxs-lookup"><span data-stu-id="6ee99-145">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="6ee99-146">Значение времени действия находится в диапазоне от 15 до 90 секунд включительно.</span><span class="sxs-lookup"><span data-stu-id="6ee99-146">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="6ee99-147">По умолчанию значение временивыполнения составляет 55 секунд для одного целевого объекта и 60 секунд для нескольких целей (при условии изменения).</span><span class="sxs-lookup"><span data-stu-id="6ee99-147">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="6ee99-148">maskCallee</span><span class="sxs-lookup"><span data-stu-id="6ee99-148">maskCallee</span></span>|<span data-ttu-id="6ee99-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ee99-149">Boolean</span></span>|<span data-ttu-id="6ee99-150">Указывает, должен ли вызываемая стороны быть скрыта от вызываемой стороны.</span><span class="sxs-lookup"><span data-stu-id="6ee99-150">Indicates whether the callee is to be hidden from the caller.</span></span> <span data-ttu-id="6ee99-151">Если установлено true, то идентификатор вызываемого пользователя — это идентификатор бота.</span><span class="sxs-lookup"><span data-stu-id="6ee99-151">If true, then the callee identity is the bot identity.</span></span> <span data-ttu-id="6ee99-152">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="6ee99-152">Default: false.</span></span>|
|<span data-ttu-id="6ee99-153">maskCaller</span><span class="sxs-lookup"><span data-stu-id="6ee99-153">maskCaller</span></span>|<span data-ttu-id="6ee99-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ee99-154">Boolean</span></span>|<span data-ttu-id="6ee99-155">Указывает, следует ли скрывать вызываемую от вызываемой стороны.</span><span class="sxs-lookup"><span data-stu-id="6ee99-155">Indicates whether the caller is to be hidden from the callee.</span></span> <span data-ttu-id="6ee99-156">Если установлено true, то идентификатором вызывающего пользователя является идентификатор бота.</span><span class="sxs-lookup"><span data-stu-id="6ee99-156">If true, then the caller identity is the bot identity.</span></span> <span data-ttu-id="6ee99-157">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="6ee99-157">Default: false.</span></span>|
|<span data-ttu-id="6ee99-158">callbackUri</span><span class="sxs-lookup"><span data-stu-id="6ee99-158">callbackUri</span></span>|<span data-ttu-id="6ee99-159">String</span><span class="sxs-lookup"><span data-stu-id="6ee99-159">String</span></span>|<span data-ttu-id="6ee99-160">Это позволяет ботам предоставлять определенный URI для текущего вызова для получения последующих уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6ee99-160">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="6ee99-161">Если это свойство не за установлено, вместо него будет использоваться глобальный URI для вызова бота.</span><span class="sxs-lookup"><span data-stu-id="6ee99-161">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="6ee99-162">Это должен быть `https` .</span><span class="sxs-lookup"><span data-stu-id="6ee99-162">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="6ee99-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee99-163">Response</span></span>
<span data-ttu-id="6ee99-164">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="6ee99-164">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6ee99-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="6ee99-165">Examples</span></span>
<span data-ttu-id="6ee99-166">В этих примерах освещается рабочий процесс уведомления о входящих вызовах и его перенаправление.</span><span class="sxs-lookup"><span data-stu-id="6ee99-166">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="6ee99-167">**Примечание.** Показанные здесь объекты ответа могут быть сокращены для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="6ee99-167">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="6ee99-168">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ee99-168">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="6ee99-169">Пример 1. Переад вызов на целевой объект</span><span class="sxs-lookup"><span data-stu-id="6ee99-169">Example 1: Forward a call to a target</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="6ee99-170">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6ee99-170">Notification - incoming</span></span>
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

#### <a name="request"></a><span data-ttu-id="6ee99-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee99-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6ee99-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ee99-172">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6ee99-173">C#</span><span class="sxs-lookup"><span data-stu-id="6ee99-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ee99-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ee99-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ee99-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ee99-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ee99-176">Java</span><span class="sxs-lookup"><span data-stu-id="6ee99-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6ee99-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee99-177">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="notification---terminated"></a><span data-ttu-id="6ee99-178">Уведомление — завершено</span><span class="sxs-lookup"><span data-stu-id="6ee99-178">Notification - terminated</span></span>

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

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="6ee99-179">Пример 2. Переадронизовыв вызов на несколько целей с одновременным вызовом</span><span class="sxs-lookup"><span data-stu-id="6ee99-179">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="6ee99-180">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6ee99-180">Notification - incoming</span></span>

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

#### <a name="request"></a><span data-ttu-id="6ee99-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee99-181">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="6ee99-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee99-182">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

#### <a name="notification---terminated"></a><span data-ttu-id="6ee99-183">Уведомление — завершено</span><span class="sxs-lookup"><span data-stu-id="6ee99-183">Notification - terminated</span></span>

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

### <a name="example-3-forward-a-call-to-a-pstn-number"></a><span data-ttu-id="6ee99-184">Пример 3. Переадронизовыв вызов на номер STN</span><span class="sxs-lookup"><span data-stu-id="6ee99-184">Example 3: Forward a call to a PSTN number</span></span>

<span data-ttu-id="6ee99-185">Для этого вызова требуется экземпляр приложения с назначенным номером STN.</span><span class="sxs-lookup"><span data-stu-id="6ee99-185">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="6ee99-186">Шаг 1. Создание экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="6ee99-186">Step 1: Create application instance</span></span>
<span data-ttu-id="6ee99-187">Используя учетные данные администратора клиента, вызовите следующие cmdlets в удаленной powerShell клиента, чтобы создать экземпляр приложения.</span><span class="sxs-lookup"><span data-stu-id="6ee99-187">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="6ee99-188">Дополнительные сведения см. в командах [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="6ee99-188">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="6ee99-189">Шаг 2. Назначение лицензий Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6ee99-189">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="6ee99-190">Используйте учетные данные администратора клиента для входа и перейдите на вкладку https://admin.microsoft.com/ **"Пользователи > активные пользователи".**</span><span class="sxs-lookup"><span data-stu-id="6ee99-190">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="6ee99-191">Выберите экземпляр приложения, назначьте план внутренних и международных звонков **Microsoft 365** и телефонную систему **Microsoft 365 —** лицензии виртуальных пользователей и нажмите кнопку **"Сохранить изменения".**</span><span class="sxs-lookup"><span data-stu-id="6ee99-191">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="6ee99-192">Если необходимые лицензии недоступны в клиенте, их можно получить на вкладке "Выставление счета **-> Приобретение служб".**</span><span class="sxs-lookup"><span data-stu-id="6ee99-192">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="6ee99-193">Шаг 3. Получение номера STN</span><span class="sxs-lookup"><span data-stu-id="6ee99-193">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="6ee99-194">Используйте учетные данные администратора клиента для входа и перейдите на вкладку "Устаревший https://admin.teams.microsoft.com/ **портал"** на левой панели.</span><span class="sxs-lookup"><span data-stu-id="6ee99-194">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="6ee99-195">На новой странице перейдите на вкладку **голосовых > номеров** телефонов.</span><span class="sxs-lookup"><span data-stu-id="6ee99-195">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="6ee99-196">Нажмите **+** кнопку, выберите **"Новые номера служб"** и перейдите на страницу **"Добавление новых номеров служб".**</span><span class="sxs-lookup"><span data-stu-id="6ee99-196">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="6ee99-197">Выберите **"Страна/регион",** **"Область",** **"Город",**"Количество **входных** данных" и нажмите **кнопку "Добавить"** для поиска.</span><span class="sxs-lookup"><span data-stu-id="6ee99-197">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="6ee99-198">Щелкните **"Получить номера".**</span><span class="sxs-lookup"><span data-stu-id="6ee99-198">Click **acquire numbers**.</span></span> <span data-ttu-id="6ee99-199">Недавно полученный номер будет показываться на **вкладке "Номера** телефонов".</span><span class="sxs-lookup"><span data-stu-id="6ee99-199">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="6ee99-200">Шаг 4. Назначение номера STN экземпляру приложения</span><span class="sxs-lookup"><span data-stu-id="6ee99-200">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="6ee99-201">С помощью учетных данных администратора клиента вызовите следующие cmdlets в удаленной powerShell клиента, чтобы назначить номер STN экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="6ee99-201">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="6ee99-202">Дополнительные сведения см. в командах [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="6ee99-202">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
> <span data-ttu-id="6ee99-203">**Примечание.** Если клиент имеет номера STN в Австралии, присвоенные экземплярам приложений, этот вызов может привести к сбойу.</span><span class="sxs-lookup"><span data-stu-id="6ee99-203">**Note:** If a tenant has Australian PSTN numbers assigned to any application instances, this call might fail.</span></span> <span data-ttu-id="6ee99-204">Если клиент создан только что, может потребоваться несколько дней, чтобы эта функция была доступна.</span><span class="sxs-lookup"><span data-stu-id="6ee99-204">If a tenant is newly created, it might take several days for this feature to be available.</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="6ee99-205">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6ee99-205">Notification - incoming</span></span>
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

#### <a name="request"></a><span data-ttu-id="6ee99-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee99-206">Request</span></span>

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
#### <a name="response"></a><span data-ttu-id="6ee99-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee99-207">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="notification---terminated"></a><span data-ttu-id="6ee99-208">Уведомление — завершено</span><span class="sxs-lookup"><span data-stu-id="6ee99-208">Notification - terminated</span></span>

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


