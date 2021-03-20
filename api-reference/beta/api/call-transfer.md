---
title: 'вызов: передача'
description: Передача активного одноранговых вызовов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f4be30fff38c639ac55d126b0501b3f9f57afa52
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948460"
---
# <a name="call-transfer"></a><span data-ttu-id="59d29-103">вызов: передача</span><span class="sxs-lookup"><span data-stu-id="59d29-103">call: transfer</span></span>

<span data-ttu-id="59d29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59d29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59d29-105">Передача активного одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="59d29-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="59d29-106">**Примечание:** Это поддерживается только в том случае, если как передателем, так и целевой целью передачи являются пользователи Microsoft Teams, принадлежащие одному клиенту.</span><span class="sxs-lookup"><span data-stu-id="59d29-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="59d29-107">Передача на номер PSTN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="59d29-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="59d29-108">Дополнительные информацию о целевой цели переноса, переноса и переноса см. в [rFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="59d29-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="59d29-109">Консультативная передача означает, что перед передачей перед передачей переносчик может сообщить человеку, на которого он хочет передать вызов.</span><span class="sxs-lookup"><span data-stu-id="59d29-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="59d29-110">Это противоположно переносу вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="59d29-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="59d29-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59d29-111">Permissions</span></span>
<span data-ttu-id="59d29-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59d29-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59d29-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59d29-114">Permission type</span></span> | <span data-ttu-id="59d29-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59d29-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="59d29-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59d29-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="59d29-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="59d29-117">Not Supported</span></span>                |
| <span data-ttu-id="59d29-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59d29-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59d29-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="59d29-119">Not Supported</span></span>                |
| <span data-ttu-id="59d29-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="59d29-120">Application</span></span>     | <span data-ttu-id="59d29-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="59d29-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="59d29-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59d29-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="59d29-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="59d29-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="59d29-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="59d29-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59d29-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59d29-125">Request headers</span></span>
| <span data-ttu-id="59d29-126">Имя</span><span class="sxs-lookup"><span data-stu-id="59d29-126">Name</span></span>          | <span data-ttu-id="59d29-127">Описание</span><span class="sxs-lookup"><span data-stu-id="59d29-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="59d29-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59d29-128">Authorization</span></span> | <span data-ttu-id="59d29-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59d29-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59d29-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59d29-131">Content-type</span></span>  | <span data-ttu-id="59d29-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59d29-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59d29-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59d29-134">Request body</span></span>
<span data-ttu-id="59d29-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="59d29-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59d29-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="59d29-136">Parameter</span></span>      | <span data-ttu-id="59d29-137">Тип</span><span class="sxs-lookup"><span data-stu-id="59d29-137">Type</span></span>    |<span data-ttu-id="59d29-138">Описание</span><span class="sxs-lookup"><span data-stu-id="59d29-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59d29-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="59d29-139">transferTarget</span></span>|[<span data-ttu-id="59d29-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="59d29-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="59d29-141">Участник, который является объектом переноса.</span><span class="sxs-lookup"><span data-stu-id="59d29-141">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="59d29-142">clientContext</span><span class="sxs-lookup"><span data-stu-id="59d29-142">clientContext</span></span>|<span data-ttu-id="59d29-143">Строка</span><span class="sxs-lookup"><span data-stu-id="59d29-143">String</span></span>|<span data-ttu-id="59d29-144">Уникальная строка Client Context.</span><span class="sxs-lookup"><span data-stu-id="59d29-144">Unique Client Context string.</span></span> <span data-ttu-id="59d29-145">Максимальное ограничение — 256 шаров.</span><span class="sxs-lookup"><span data-stu-id="59d29-145">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="59d29-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d29-146">Response</span></span>
<span data-ttu-id="59d29-147">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="59d29-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="59d29-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="59d29-148">Examples</span></span>
<span data-ttu-id="59d29-149">В этих примерах покажите поток входящих вызовов в различные типы уведомлений о переносе.</span><span class="sxs-lookup"><span data-stu-id="59d29-149">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="59d29-150">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="59d29-150">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="59d29-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d29-151">Request</span></span>
<span data-ttu-id="59d29-152">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59d29-152">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="59d29-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="59d29-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-1"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="c"></a>[<span data-ttu-id="59d29-154">C#</span><span class="sxs-lookup"><span data-stu-id="59d29-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59d29-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59d29-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59d29-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59d29-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="59d29-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d29-157">Response</span></span>

> <span data-ttu-id="59d29-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59d29-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="59d29-160">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="59d29-160">Notification - transferring</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="59d29-161">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="59d29-161">Notification - transfer accepted</span></span>

> <span data-ttu-id="59d29-162">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="59d29-162">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

#### <a name="notification---transfer-completed"></a><span data-ttu-id="59d29-163">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="59d29-163">Notification - transfer completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 0,
          "subcode": 7015,
          "message": "GracefulTransferCompleted"
        }
      }
    }
  ]
}
```

#### <a name="notification---transfer-failed"></a><span data-ttu-id="59d29-164">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="59d29-164">Notification - transfer failed</span></span>

> <span data-ttu-id="59d29-165">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="59d29-165">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7000,
          "message": "<message>"
        }
      }
    }
  ]
}
```

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="59d29-166">Пример 2. Перенос консультаций</span><span class="sxs-lookup"><span data-stu-id="59d29-166">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="59d29-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d29-167">Request</span></span>
<span data-ttu-id="59d29-168">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59d29-168">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer-2"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
Content-Type: application/json

{
  "transferTarget": {
    "@odata.type": "#microsoft.graph.invitationParticipantInfo",
    "endpointType": "default",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-us",
    "region": "amer",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

#### <a name="response"></a><span data-ttu-id="59d29-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d29-169">Response</span></span>

> <span data-ttu-id="59d29-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59d29-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="59d29-172">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="59d29-172">Notification - transferring</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="59d29-173">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="59d29-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="59d29-174">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="59d29-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

#### <a name="notification---transfer-completed"></a><span data-ttu-id="59d29-175">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="59d29-175">Notification - transfer completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

#### <a name="notification---transfer-failed"></a><span data-ttu-id="59d29-176">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="59d29-176">Notification - transfer failed</span></span>

> <span data-ttu-id="59d29-177">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="59d29-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7700,
          "message": "<message>"
        },
        "replacesContext": "<replacesContext>"
      }
    }
  ]
}
```

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="59d29-178">Пример 3. Передача вызовов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="59d29-178">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="59d29-179">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="59d29-179">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="59d29-180">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="59d29-180">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="59d29-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d29-181">Request</span></span>
<span data-ttu-id="59d29-182">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59d29-182">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-transfer"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

#### <a name="response"></a><span data-ttu-id="59d29-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d29-183">Response</span></span>

> <span data-ttu-id="59d29-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59d29-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="59d29-186">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="59d29-186">Notification - transferring</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="59d29-187">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="59d29-187">Notification - transfer accepted</span></span>

> <span data-ttu-id="59d29-188">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="59d29-188">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

#### <a name="notification---transfer-completed"></a><span data-ttu-id="59d29-189">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="59d29-189">Notification - transfer completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 0,
          "subcode": 7015,
          "message": "GracefulTransferCompleted"
        }
      }
    }
  ]
}
```
### <a name="notification---transfer-failed"></a><span data-ttu-id="59d29-190">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="59d29-190">Notification - transfer failed</span></span>

> <span data-ttu-id="59d29-191">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="59d29-191">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7000,
          "message": "<message>"
        }
      }
    }
  ]
}
```

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="59d29-192">Пример 4. Консультативный перевод на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="59d29-192">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="59d29-193">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="59d29-193">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="59d29-194">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="59d29-194">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="59d29-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d29-195">Request</span></span>
<span data-ttu-id="59d29-196">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59d29-196">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
Content-Type: application/json

{
  "transferTarget": {
    "@odata.type": "#microsoft.graph.invitationParticipantInfo",
    "endpointType": "default",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
    },
    "languageId": "en-us",
    "region": "amer",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

#### <a name="response"></a><span data-ttu-id="59d29-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d29-197">Response</span></span>

> <span data-ttu-id="59d29-p113">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59d29-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="59d29-200">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="59d29-200">Notification - transferring</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="59d29-201">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="59d29-201">Notification - transfer accepted</span></span>

> <span data-ttu-id="59d29-202">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="59d29-202">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

#### <a name="notification---transfer-completed"></a><span data-ttu-id="59d29-203">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="59d29-203">Notification - transfer completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

#### <a name="notification---transfer-failed"></a><span data-ttu-id="59d29-204">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="59d29-204">Notification - transfer failed</span></span>

> <span data-ttu-id="59d29-205">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="59d29-205">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7700,
          "message": "<message>"
        }
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
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


