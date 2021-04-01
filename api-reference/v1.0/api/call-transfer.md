---
title: 'вызов: передача'
description: Передача активного одноранговых вызовов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 59b009aed4440fd30a4b038bc4eb40eba208c5ef
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473446"
---
# <a name="call-transfer"></a><span data-ttu-id="12a2f-103">вызов: передача</span><span class="sxs-lookup"><span data-stu-id="12a2f-103">call: transfer</span></span>

<span data-ttu-id="12a2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12a2f-105">Передача активного одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="12a2f-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="12a2f-106">**Примечание:** Это поддерживается только в том случае, если как передателем, так и целевой целью передачи являются пользователи Microsoft Teams, принадлежащие одному клиенту.</span><span class="sxs-lookup"><span data-stu-id="12a2f-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="12a2f-107">Передача на номер PSTN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="12a2f-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="12a2f-108">Дополнительные информацию о целевой цели переноса, переноса и переноса см. в [rFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="12a2f-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="12a2f-109">Консультативная передача означает, что перед передачей перед передачей переносчик может сообщить человеку, на которого он хочет передать вызов.</span><span class="sxs-lookup"><span data-stu-id="12a2f-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="12a2f-110">Это противоположно переносу вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="12a2f-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="12a2f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12a2f-111">Permissions</span></span>
<span data-ttu-id="12a2f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12a2f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12a2f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12a2f-114">Permission type</span></span> | <span data-ttu-id="12a2f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12a2f-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="12a2f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12a2f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="12a2f-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12a2f-117">Not Supported</span></span>                |
| <span data-ttu-id="12a2f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12a2f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12a2f-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12a2f-119">Not Supported</span></span>                |
| <span data-ttu-id="12a2f-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12a2f-120">Application</span></span>     | <span data-ttu-id="12a2f-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="12a2f-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="12a2f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12a2f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="12a2f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12a2f-123">Request headers</span></span>
| <span data-ttu-id="12a2f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="12a2f-124">Name</span></span>          | <span data-ttu-id="12a2f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="12a2f-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="12a2f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12a2f-126">Authorization</span></span> | <span data-ttu-id="12a2f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12a2f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12a2f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12a2f-129">Content-type</span></span>  | <span data-ttu-id="12a2f-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12a2f-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12a2f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12a2f-132">Request body</span></span>
<span data-ttu-id="12a2f-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="12a2f-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="12a2f-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="12a2f-134">Parameter</span></span>      | <span data-ttu-id="12a2f-135">Тип</span><span class="sxs-lookup"><span data-stu-id="12a2f-135">Type</span></span>    |<span data-ttu-id="12a2f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="12a2f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12a2f-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="12a2f-137">transferTarget</span></span>|[<span data-ttu-id="12a2f-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="12a2f-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="12a2f-139">Участник, который является объектом переноса.</span><span class="sxs-lookup"><span data-stu-id="12a2f-139">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="12a2f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a2f-140">Response</span></span>
<span data-ttu-id="12a2f-141">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="12a2f-141">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="12a2f-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="12a2f-142">Examples</span></span>
<span data-ttu-id="12a2f-143">В этих примерах покажите поток входящих вызовов в различные типы уведомлений о переносе.</span><span class="sxs-lookup"><span data-stu-id="12a2f-143">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="12a2f-144">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="12a2f-144">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="12a2f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a2f-145">Request</span></span>
<span data-ttu-id="12a2f-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a2f-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="12a2f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="12a2f-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="12a2f-148">C#</span><span class="sxs-lookup"><span data-stu-id="12a2f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12a2f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12a2f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12a2f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12a2f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12a2f-151">Java</span><span class="sxs-lookup"><span data-stu-id="12a2f-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="12a2f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a2f-152">Response</span></span>

> <span data-ttu-id="12a2f-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12a2f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="12a2f-155">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="12a2f-155">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="12a2f-156">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="12a2f-156">Notification - transfer accepted</span></span>

> <span data-ttu-id="12a2f-157">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="12a2f-157">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="12a2f-158">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="12a2f-158">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="12a2f-159">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="12a2f-159">Notification - transfer failed</span></span>

> <span data-ttu-id="12a2f-160">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="12a2f-160">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="12a2f-161">Пример 2. Перенос консультаций</span><span class="sxs-lookup"><span data-stu-id="12a2f-161">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="12a2f-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a2f-162">Request</span></span>
<span data-ttu-id="12a2f-163">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a2f-163">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer-2"
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

##### <a name="response"></a><span data-ttu-id="12a2f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a2f-164">Response</span></span>

> <span data-ttu-id="12a2f-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12a2f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="12a2f-167">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="12a2f-167">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="12a2f-168">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="12a2f-168">Notification - transfer accepted</span></span>

> <span data-ttu-id="12a2f-169">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="12a2f-169">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="12a2f-170">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="12a2f-170">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="12a2f-171">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="12a2f-171">Notification - transfer failed</span></span>

> <span data-ttu-id="12a2f-172">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="12a2f-172">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="12a2f-173">Пример 3. Передача вызовов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="12a2f-173">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="12a2f-174">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="12a2f-174">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="12a2f-175">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="12a2f-175">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="12a2f-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a2f-176">Request</span></span>
<span data-ttu-id="12a2f-177">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a2f-177">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="12a2f-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a2f-178">Response</span></span>

> <span data-ttu-id="12a2f-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12a2f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="12a2f-181">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="12a2f-181">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="12a2f-182">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="12a2f-182">Notification - transfer accepted</span></span>

> <span data-ttu-id="12a2f-183">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="12a2f-183">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="12a2f-184">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="12a2f-184">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="12a2f-185">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="12a2f-185">Notification - transfer failed</span></span>

> <span data-ttu-id="12a2f-186">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="12a2f-186">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="12a2f-187">Пример 4. Консультативный перевод на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="12a2f-187">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="12a2f-188">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="12a2f-188">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="12a2f-189">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="12a2f-189">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="12a2f-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a2f-190">Request</span></span>
<span data-ttu-id="12a2f-191">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a2f-191">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="12a2f-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a2f-192">Response</span></span>

> <span data-ttu-id="12a2f-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12a2f-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="12a2f-195">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="12a2f-195">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="12a2f-196">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="12a2f-196">Notification - transfer accepted</span></span>

> <span data-ttu-id="12a2f-197">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="12a2f-197">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="12a2f-198">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="12a2f-198">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="12a2f-199">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="12a2f-199">Notification - transfer failed</span></span>

> <span data-ttu-id="12a2f-200">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="12a2f-200">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

