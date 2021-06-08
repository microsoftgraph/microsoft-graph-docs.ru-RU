---
title: 'вызов: передача'
description: Передача активного одноранговых вызовов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2214d4276fc16c198ced411fe125e13389be3480
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52784915"
---
# <a name="call-transfer"></a><span data-ttu-id="ecaeb-103">вызов: передача</span><span class="sxs-lookup"><span data-stu-id="ecaeb-103">call: transfer</span></span>

<span data-ttu-id="ecaeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecaeb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecaeb-105">Передача активного одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="ecaeb-106">**Примечание:** Это поддерживается только в том случае, если как передателем, так и Microsoft Teams пользователями, принадлежащими одному и одному клиенту.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="ecaeb-107">Передача на номер PSTN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="ecaeb-108">Дополнительные информацию о целевой цели переноса, переноса и переноса см. в [rFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="ecaeb-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="ecaeb-109">Консультативная передача означает, что перед передачей перед передачей переносчик может сообщить человеку, на которого он хочет передать вызов.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="ecaeb-110">Это противоположно переносу вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecaeb-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecaeb-111">Permissions</span></span>
<span data-ttu-id="ecaeb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecaeb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecaeb-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecaeb-114">Permission type</span></span> | <span data-ttu-id="ecaeb-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecaeb-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="ecaeb-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecaeb-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="ecaeb-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ecaeb-117">Not Supported</span></span>                |
| <span data-ttu-id="ecaeb-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecaeb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecaeb-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ecaeb-119">Not Supported</span></span>                |
| <span data-ttu-id="ecaeb-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecaeb-120">Application</span></span>     | <span data-ttu-id="ecaeb-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="ecaeb-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="ecaeb-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecaeb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="ecaeb-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecaeb-123">Request headers</span></span>
| <span data-ttu-id="ecaeb-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ecaeb-124">Name</span></span>          | <span data-ttu-id="ecaeb-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ecaeb-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ecaeb-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecaeb-126">Authorization</span></span> | <span data-ttu-id="ecaeb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ecaeb-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ecaeb-129">Content-type</span></span>  | <span data-ttu-id="ecaeb-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecaeb-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecaeb-132">Request body</span></span>
<span data-ttu-id="ecaeb-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ecaeb-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="ecaeb-134">Parameter</span></span>      | <span data-ttu-id="ecaeb-135">Тип</span><span class="sxs-lookup"><span data-stu-id="ecaeb-135">Type</span></span>    |<span data-ttu-id="ecaeb-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ecaeb-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecaeb-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="ecaeb-137">transferTarget</span></span>|[<span data-ttu-id="ecaeb-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="ecaeb-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="ecaeb-139">Участник, который является объектом переноса.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-139">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="ecaeb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecaeb-140">Response</span></span>
<span data-ttu-id="ecaeb-141">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-141">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ecaeb-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="ecaeb-142">Examples</span></span>
<span data-ttu-id="ecaeb-143">В этих примерах покажите поток входящих вызовов в различные типы уведомлений о переносе.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-143">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="ecaeb-144">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="ecaeb-144">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="ecaeb-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecaeb-145">Request</span></span>
<span data-ttu-id="ecaeb-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ecaeb-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecaeb-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-1"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "displayName": "Heidi Steen"
      }
    },
    "replacesCallId": "replacesCallId-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ecaeb-148">C#</span><span class="sxs-lookup"><span data-stu-id="ecaeb-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecaeb-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecaeb-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecaeb-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecaeb-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecaeb-151">Java</span><span class="sxs-lookup"><span data-stu-id="ecaeb-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ecaeb-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecaeb-152">Response</span></span>

> <span data-ttu-id="ecaeb-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="ecaeb-154">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="ecaeb-154">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="ecaeb-155">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="ecaeb-155">Notification - transfer accepted</span></span>

> <span data-ttu-id="ecaeb-156">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-156">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="ecaeb-157">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="ecaeb-157">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="ecaeb-158">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="ecaeb-158">Notification - transfer failed</span></span>

> <span data-ttu-id="ecaeb-159">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="ecaeb-159">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
        },
        "replacesContext": "<replacesContext>"
      }
    }
  ]
}
```

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="ecaeb-160">Пример 2. Перенос консультаций</span><span class="sxs-lookup"><span data-stu-id="ecaeb-160">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="ecaeb-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecaeb-161">Request</span></span>
<span data-ttu-id="ecaeb-162">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-162">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ecaeb-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecaeb-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-2"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
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
        "displayName": "Heidi Steen"
      }
    },
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ecaeb-164">C#</span><span class="sxs-lookup"><span data-stu-id="ecaeb-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecaeb-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecaeb-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecaeb-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecaeb-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ecaeb-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecaeb-167">Response</span></span>

> <span data-ttu-id="ecaeb-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-168">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="ecaeb-169">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="ecaeb-169">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="ecaeb-170">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="ecaeb-170">Notification - transfer accepted</span></span>

> <span data-ttu-id="ecaeb-171">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-171">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="ecaeb-172">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="ecaeb-172">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="ecaeb-173">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="ecaeb-173">Notification - transfer failed</span></span>

> <span data-ttu-id="ecaeb-174">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="ecaeb-174">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="ecaeb-175">Пример 3. Передача вызовов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="ecaeb-175">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="ecaeb-176">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-176">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="ecaeb-177">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="ecaeb-177">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="ecaeb-178">**Примечание.** Телефон ID — это номер телефона в формате E.164.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-178">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="ecaeb-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecaeb-179">Request</span></span>
<span data-ttu-id="ecaeb-180">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-180">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ecaeb-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecaeb-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-3"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/transfer
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
# <a name="javascript"></a>[<span data-ttu-id="ecaeb-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecaeb-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ecaeb-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecaeb-183">Response</span></span>

> <span data-ttu-id="ecaeb-184">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-184">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="ecaeb-185">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="ecaeb-185">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="ecaeb-186">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="ecaeb-186">Notification - transfer accepted</span></span>

> <span data-ttu-id="ecaeb-187">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-187">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="ecaeb-188">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="ecaeb-188">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="ecaeb-189">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="ecaeb-189">Notification - transfer failed</span></span>

> <span data-ttu-id="ecaeb-190">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="ecaeb-190">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="ecaeb-191">Пример 4. Консультативный перевод на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="ecaeb-191">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="ecaeb-192">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-192">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="ecaeb-193">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="ecaeb-193">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="ecaeb-194">**Примечание.** Телефон ID — это номер телефона в формате E.164.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-194">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="ecaeb-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecaeb-195">Request</span></span>
<span data-ttu-id="ecaeb-196">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-196">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ecaeb-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecaeb-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-4"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
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
# <a name="javascript"></a>[<span data-ttu-id="ecaeb-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecaeb-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ecaeb-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecaeb-199">Response</span></span>

> <span data-ttu-id="ecaeb-200">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-200">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="ecaeb-201">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="ecaeb-201">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="ecaeb-202">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="ecaeb-202">Notification - transfer accepted</span></span>

> <span data-ttu-id="ecaeb-203">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="ecaeb-203">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="ecaeb-204">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="ecaeb-204">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="ecaeb-205">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="ecaeb-205">Notification - transfer failed</span></span>

> <span data-ttu-id="ecaeb-206">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="ecaeb-206">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

