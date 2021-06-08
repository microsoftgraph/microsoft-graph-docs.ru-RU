---
title: 'вызов: передача'
description: Передача активного одноранговых вызовов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6b4a9c00bc40f2bfd0ea9cc40317c426f2c2aa2c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786561"
---
# <a name="call-transfer"></a><span data-ttu-id="4218e-103">вызов: передача</span><span class="sxs-lookup"><span data-stu-id="4218e-103">call: transfer</span></span>

<span data-ttu-id="4218e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4218e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4218e-105">Передача активного одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="4218e-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="4218e-106">**Примечание:** Это поддерживается только в том случае, если как передателем, так и Microsoft Teams пользователями, принадлежащими одному и одному клиенту.</span><span class="sxs-lookup"><span data-stu-id="4218e-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="4218e-107">Передача на номер PSTN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="4218e-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="4218e-108">Дополнительные информацию о целевой цели переноса, переноса и переноса см. в [rFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="4218e-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="4218e-109">Консультативная передача означает, что перед передачей перед передачей переносчик может сообщить человеку, на которого он хочет передать вызов.</span><span class="sxs-lookup"><span data-stu-id="4218e-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="4218e-110">Это противоположно переносу вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="4218e-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="4218e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4218e-111">Permissions</span></span>
<span data-ttu-id="4218e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4218e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4218e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4218e-114">Permission type</span></span> | <span data-ttu-id="4218e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4218e-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="4218e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4218e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="4218e-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4218e-117">Not Supported</span></span>                |
| <span data-ttu-id="4218e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4218e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4218e-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4218e-119">Not Supported</span></span>                |
| <span data-ttu-id="4218e-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="4218e-120">Application</span></span>     | <span data-ttu-id="4218e-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="4218e-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="4218e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4218e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="4218e-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="4218e-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="4218e-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="4218e-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4218e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4218e-125">Request headers</span></span>
| <span data-ttu-id="4218e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="4218e-126">Name</span></span>          | <span data-ttu-id="4218e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4218e-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4218e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4218e-128">Authorization</span></span> | <span data-ttu-id="4218e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4218e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4218e-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4218e-131">Content-type</span></span>  | <span data-ttu-id="4218e-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4218e-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4218e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4218e-134">Request body</span></span>
<span data-ttu-id="4218e-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4218e-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4218e-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="4218e-136">Parameter</span></span>      | <span data-ttu-id="4218e-137">Тип</span><span class="sxs-lookup"><span data-stu-id="4218e-137">Type</span></span>    |<span data-ttu-id="4218e-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4218e-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4218e-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="4218e-139">transferTarget</span></span>|[<span data-ttu-id="4218e-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="4218e-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="4218e-141">Участник, который является объектом переноса.</span><span class="sxs-lookup"><span data-stu-id="4218e-141">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="4218e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4218e-142">Response</span></span>
<span data-ttu-id="4218e-143">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="4218e-143">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4218e-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="4218e-144">Examples</span></span>
<span data-ttu-id="4218e-145">В этих примерах покажите поток входящих вызовов в различные типы уведомлений о переносе.</span><span class="sxs-lookup"><span data-stu-id="4218e-145">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="4218e-146">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="4218e-146">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="4218e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4218e-147">Request</span></span>
<span data-ttu-id="4218e-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4218e-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4218e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="4218e-149">HTTP</span></span>](#tab/http)
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4218e-150">C#</span><span class="sxs-lookup"><span data-stu-id="4218e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4218e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4218e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4218e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4218e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4218e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4218e-153">Response</span></span>

> <span data-ttu-id="4218e-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4218e-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="4218e-155">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="4218e-155">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="4218e-156">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="4218e-156">Notification - transfer accepted</span></span>

> <span data-ttu-id="4218e-157">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4218e-157">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="4218e-158">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="4218e-158">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="4218e-159">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="4218e-159">Notification - transfer failed</span></span>

> <span data-ttu-id="4218e-160">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="4218e-160">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="4218e-161">Пример 2. Перенос консультаций</span><span class="sxs-lookup"><span data-stu-id="4218e-161">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="4218e-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="4218e-162">Request</span></span>
<span data-ttu-id="4218e-163">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4218e-163">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4218e-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="4218e-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-2"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4218e-165">C#</span><span class="sxs-lookup"><span data-stu-id="4218e-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4218e-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4218e-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4218e-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4218e-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4218e-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="4218e-168">Response</span></span>

> <span data-ttu-id="4218e-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4218e-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="4218e-170">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="4218e-170">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="4218e-171">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="4218e-171">Notification - transfer accepted</span></span>

> <span data-ttu-id="4218e-172">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4218e-172">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="4218e-173">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="4218e-173">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="4218e-174">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="4218e-174">Notification - transfer failed</span></span>

> <span data-ttu-id="4218e-175">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="4218e-175">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="4218e-176">Пример 3. Передача вызовов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="4218e-176">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="4218e-177">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="4218e-177">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="4218e-178">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="4218e-178">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="4218e-179">**Примечание.** Телефон ID — это номер телефона в формате E.164.</span><span class="sxs-lookup"><span data-stu-id="4218e-179">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="4218e-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="4218e-180">Request</span></span>
<span data-ttu-id="4218e-181">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4218e-181">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4218e-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="4218e-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-3"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4218e-183">C#</span><span class="sxs-lookup"><span data-stu-id="4218e-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4218e-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4218e-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4218e-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="4218e-185">Response</span></span>

> <span data-ttu-id="4218e-186">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4218e-186">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="4218e-187">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="4218e-187">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="4218e-188">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="4218e-188">Notification - transfer accepted</span></span>

> <span data-ttu-id="4218e-189">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4218e-189">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="4218e-190">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="4218e-190">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="4218e-191">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="4218e-191">Notification - transfer failed</span></span>

> <span data-ttu-id="4218e-192">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="4218e-192">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="4218e-193">Пример 4. Консультативный перевод на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="4218e-193">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="4218e-194">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="4218e-194">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="4218e-195">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="4218e-195">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="4218e-196">**Примечание.** Телефон ID — это номер телефона в формате E.164.</span><span class="sxs-lookup"><span data-stu-id="4218e-196">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="4218e-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="4218e-197">Request</span></span>
<span data-ttu-id="4218e-198">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4218e-198">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4218e-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="4218e-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-4"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4218e-200">C#</span><span class="sxs-lookup"><span data-stu-id="4218e-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4218e-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4218e-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4218e-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="4218e-202">Response</span></span>

> <span data-ttu-id="4218e-203">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4218e-203">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="4218e-204">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="4218e-204">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="4218e-205">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="4218e-205">Notification - transfer accepted</span></span>

> <span data-ttu-id="4218e-206">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4218e-206">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="4218e-207">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="4218e-207">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="4218e-208">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="4218e-208">Notification - transfer failed</span></span>

> <span data-ttu-id="4218e-209">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="4218e-209">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


