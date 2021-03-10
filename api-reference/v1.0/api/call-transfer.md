---
title: 'вызов: передача'
description: Передача активного одноранговых вызовов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2feec9b37375da3b76191ec84869346c07af36f3
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573770"
---
# <a name="call-transfer"></a><span data-ttu-id="2f563-103">вызов: передача</span><span class="sxs-lookup"><span data-stu-id="2f563-103">call: transfer</span></span>

<span data-ttu-id="2f563-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f563-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f563-105">Передача активного одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="2f563-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="2f563-106">**Примечание:** Это поддерживается только в том случае, если как передателем, так и целевой целью передачи являются пользователи Microsoft Teams, принадлежащие одному клиенту.</span><span class="sxs-lookup"><span data-stu-id="2f563-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="2f563-107">Передача на номер PSTN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="2f563-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="2f563-108">Дополнительные информацию о целевой цели переноса, переноса и переноса см. в [rFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="2f563-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="2f563-109">Консультативная передача означает, что перед передачей перед передачей переносчик может сообщить человеку, на которого он хочет передать вызов.</span><span class="sxs-lookup"><span data-stu-id="2f563-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="2f563-110">Это противоположно переносу вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="2f563-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f563-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f563-111">Permissions</span></span>
<span data-ttu-id="2f563-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f563-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f563-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f563-114">Permission type</span></span> | <span data-ttu-id="2f563-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f563-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="2f563-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f563-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f563-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2f563-117">Not Supported</span></span>                |
| <span data-ttu-id="2f563-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f563-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f563-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2f563-119">Not Supported</span></span>                |
| <span data-ttu-id="2f563-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="2f563-120">Application</span></span>     | <span data-ttu-id="2f563-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="2f563-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="2f563-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f563-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="2f563-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f563-123">Request headers</span></span>
| <span data-ttu-id="2f563-124">Имя</span><span class="sxs-lookup"><span data-stu-id="2f563-124">Name</span></span>          | <span data-ttu-id="2f563-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2f563-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2f563-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f563-126">Authorization</span></span> | <span data-ttu-id="2f563-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f563-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f563-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f563-129">Content-type</span></span>  | <span data-ttu-id="2f563-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f563-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f563-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f563-132">Request body</span></span>
<span data-ttu-id="2f563-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2f563-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f563-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="2f563-134">Parameter</span></span>      | <span data-ttu-id="2f563-135">Тип</span><span class="sxs-lookup"><span data-stu-id="2f563-135">Type</span></span>    |<span data-ttu-id="2f563-136">Описание</span><span class="sxs-lookup"><span data-stu-id="2f563-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f563-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="2f563-137">transferTarget</span></span>|[<span data-ttu-id="2f563-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="2f563-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="2f563-139">Участник, который является объектом переноса.</span><span class="sxs-lookup"><span data-stu-id="2f563-139">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="2f563-140">clientContext</span><span class="sxs-lookup"><span data-stu-id="2f563-140">clientContext</span></span>|<span data-ttu-id="2f563-141">String</span><span class="sxs-lookup"><span data-stu-id="2f563-141">String</span></span>|<span data-ttu-id="2f563-142">Уникальная строка Client Context.</span><span class="sxs-lookup"><span data-stu-id="2f563-142">Unique Client Context string.</span></span> <span data-ttu-id="2f563-143">Максимальное ограничение — 256 шаров.</span><span class="sxs-lookup"><span data-stu-id="2f563-143">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="2f563-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f563-144">Response</span></span>
<span data-ttu-id="2f563-145">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="2f563-145">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2f563-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="2f563-146">Examples</span></span>
<span data-ttu-id="2f563-147">В этих примерах покажите поток входящих вызовов в различные типы уведомлений о переносе.</span><span class="sxs-lookup"><span data-stu-id="2f563-147">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="2f563-148">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="2f563-148">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="2f563-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f563-149">Request</span></span>
<span data-ttu-id="2f563-150">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f563-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f563-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f563-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer"
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
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="c"></a>[<span data-ttu-id="2f563-152">C#</span><span class="sxs-lookup"><span data-stu-id="2f563-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f563-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f563-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f563-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f563-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f563-155">Java</span><span class="sxs-lookup"><span data-stu-id="2f563-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2f563-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f563-156">Response</span></span>

> <span data-ttu-id="2f563-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f563-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="2f563-159">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="2f563-159">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="2f563-160">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="2f563-160">Notification - transfer accepted</span></span>

> <span data-ttu-id="2f563-161">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="2f563-161">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="2f563-162">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="2f563-162">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="2f563-163">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="2f563-163">Notification - transfer failed</span></span>

> <span data-ttu-id="2f563-164">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="2f563-164">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="2f563-165">Пример 2. Перенос консультаций</span><span class="sxs-lookup"><span data-stu-id="2f563-165">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="2f563-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f563-166">Request</span></span>
<span data-ttu-id="2f563-167">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f563-167">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer"
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
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

##### <a name="response"></a><span data-ttu-id="2f563-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f563-168">Response</span></span>

> <span data-ttu-id="2f563-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f563-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="2f563-171">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="2f563-171">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="2f563-172">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="2f563-172">Notification - transfer accepted</span></span>

> <span data-ttu-id="2f563-173">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="2f563-173">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="2f563-174">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="2f563-174">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="2f563-175">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="2f563-175">Notification - transfer failed</span></span>

> <span data-ttu-id="2f563-176">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="2f563-176">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="2f563-177">Пример 3. Передача вызовов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="2f563-177">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="2f563-178">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="2f563-178">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="2f563-179">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="2f563-179">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="2f563-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f563-180">Request</span></span>
<span data-ttu-id="2f563-181">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f563-181">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-transfer"
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

#### <a name="response"></a><span data-ttu-id="2f563-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f563-182">Response</span></span>

> <span data-ttu-id="2f563-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f563-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="2f563-185">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="2f563-185">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="2f563-186">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="2f563-186">Notification - transfer accepted</span></span>

> <span data-ttu-id="2f563-187">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="2f563-187">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="2f563-188">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="2f563-188">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="2f563-189">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="2f563-189">Notification - transfer failed</span></span>

> <span data-ttu-id="2f563-190">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="2f563-190">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="2f563-191">Пример 4. Консультативный перевод на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="2f563-191">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="2f563-192">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="2f563-192">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="2f563-193">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="2f563-193">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="2f563-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f563-194">Request</span></span>
<span data-ttu-id="2f563-195">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f563-195">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer"
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

#### <a name="response"></a><span data-ttu-id="2f563-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f563-196">Response</span></span>

> <span data-ttu-id="2f563-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f563-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="2f563-199">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="2f563-199">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="2f563-200">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="2f563-200">Notification - transfer accepted</span></span>

> <span data-ttu-id="2f563-201">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="2f563-201">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="2f563-202">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="2f563-202">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="2f563-203">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="2f563-203">Notification - transfer failed</span></span>

> <span data-ttu-id="2f563-204">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="2f563-204">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

