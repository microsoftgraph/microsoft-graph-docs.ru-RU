---
title: 'вызов: передача'
description: Передача активного одноранговых вызовов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6dc4aff080d150ae964ab2165ccfccca7c1f407a
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869738"
---
# <a name="call-transfer"></a><span data-ttu-id="bd909-103">вызов: передача</span><span class="sxs-lookup"><span data-stu-id="bd909-103">call: transfer</span></span>

<span data-ttu-id="bd909-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd909-105">Передача активного одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="bd909-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="bd909-106">**Примечание:** Это поддерживается только в том случае, если как передателем, так и целевой целью передачи являются пользователи Microsoft Teams, принадлежащие одному клиенту.</span><span class="sxs-lookup"><span data-stu-id="bd909-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="bd909-107">Передача на номер PSTN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="bd909-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="bd909-108">Дополнительные информацию о целевой цели переноса, переноса и переноса см. в [rFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="bd909-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="bd909-109">Консультативная передача означает, что перед передачей перед передачей переносчик может сообщить человеку, на которого он хочет передать вызов.</span><span class="sxs-lookup"><span data-stu-id="bd909-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="bd909-110">Это противоположно переносу вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="bd909-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd909-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd909-111">Permissions</span></span>
<span data-ttu-id="bd909-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd909-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd909-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd909-114">Permission type</span></span> | <span data-ttu-id="bd909-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd909-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="bd909-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd909-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd909-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bd909-117">Not Supported</span></span>                |
| <span data-ttu-id="bd909-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd909-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd909-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bd909-119">Not Supported</span></span>                |
| <span data-ttu-id="bd909-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd909-120">Application</span></span>     | <span data-ttu-id="bd909-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="bd909-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="bd909-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd909-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="bd909-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="bd909-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="bd909-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="bd909-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd909-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd909-125">Request headers</span></span>
| <span data-ttu-id="bd909-126">Имя</span><span class="sxs-lookup"><span data-stu-id="bd909-126">Name</span></span>          | <span data-ttu-id="bd909-127">Описание</span><span class="sxs-lookup"><span data-stu-id="bd909-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bd909-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd909-128">Authorization</span></span> | <span data-ttu-id="bd909-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd909-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd909-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd909-131">Content-type</span></span>  | <span data-ttu-id="bd909-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd909-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd909-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd909-134">Request body</span></span>
<span data-ttu-id="bd909-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bd909-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bd909-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="bd909-136">Parameter</span></span>      | <span data-ttu-id="bd909-137">Тип</span><span class="sxs-lookup"><span data-stu-id="bd909-137">Type</span></span>    |<span data-ttu-id="bd909-138">Описание</span><span class="sxs-lookup"><span data-stu-id="bd909-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd909-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="bd909-139">transferTarget</span></span>|[<span data-ttu-id="bd909-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="bd909-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="bd909-141">Участник, который является объектом переноса.</span><span class="sxs-lookup"><span data-stu-id="bd909-141">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="bd909-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd909-142">Response</span></span>
<span data-ttu-id="bd909-143">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="bd909-143">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bd909-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="bd909-144">Examples</span></span>
<span data-ttu-id="bd909-145">В этих примерах покажите поток входящих вызовов в различные типы уведомлений о переносе.</span><span class="sxs-lookup"><span data-stu-id="bd909-145">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="bd909-146">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="bd909-146">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="bd909-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd909-147">Request</span></span>
<span data-ttu-id="bd909-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd909-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bd909-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd909-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bd909-150">C#</span><span class="sxs-lookup"><span data-stu-id="bd909-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd909-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd909-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd909-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd909-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bd909-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd909-153">Response</span></span>

> <span data-ttu-id="bd909-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd909-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="bd909-156">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="bd909-156">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="bd909-157">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="bd909-157">Notification - transfer accepted</span></span>

> <span data-ttu-id="bd909-158">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="bd909-158">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="bd909-159">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="bd909-159">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="bd909-160">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="bd909-160">Notification - transfer failed</span></span>

> <span data-ttu-id="bd909-161">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="bd909-161">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="bd909-162">Пример 2. Перенос консультаций</span><span class="sxs-lookup"><span data-stu-id="bd909-162">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="bd909-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd909-163">Request</span></span>
<span data-ttu-id="bd909-164">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd909-164">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="bd909-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd909-165">Response</span></span>

> <span data-ttu-id="bd909-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd909-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="bd909-168">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="bd909-168">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="bd909-169">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="bd909-169">Notification - transfer accepted</span></span>

> <span data-ttu-id="bd909-170">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="bd909-170">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="bd909-171">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="bd909-171">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="bd909-172">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="bd909-172">Notification - transfer failed</span></span>

> <span data-ttu-id="bd909-173">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="bd909-173">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="bd909-174">Пример 3. Передача вызовов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="bd909-174">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="bd909-175">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="bd909-175">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="bd909-176">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="bd909-176">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="bd909-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd909-177">Request</span></span>
<span data-ttu-id="bd909-178">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd909-178">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="bd909-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd909-179">Response</span></span>

> <span data-ttu-id="bd909-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd909-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="bd909-182">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="bd909-182">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="bd909-183">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="bd909-183">Notification - transfer accepted</span></span>

> <span data-ttu-id="bd909-184">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="bd909-184">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="bd909-185">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="bd909-185">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="bd909-186">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="bd909-186">Notification - transfer failed</span></span>

> <span data-ttu-id="bd909-187">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="bd909-187">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="bd909-188">Пример 4. Консультативный перевод на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="bd909-188">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="bd909-189">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="bd909-189">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="bd909-190">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="bd909-190">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="bd909-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd909-191">Request</span></span>
<span data-ttu-id="bd909-192">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd909-192">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="bd909-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd909-193">Response</span></span>

> <span data-ttu-id="bd909-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd909-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="bd909-196">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="bd909-196">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="bd909-197">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="bd909-197">Notification - transfer accepted</span></span>

> <span data-ttu-id="bd909-198">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="bd909-198">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="bd909-199">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="bd909-199">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="bd909-200">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="bd909-200">Notification - transfer failed</span></span>

> <span data-ttu-id="bd909-201">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="bd909-201">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


