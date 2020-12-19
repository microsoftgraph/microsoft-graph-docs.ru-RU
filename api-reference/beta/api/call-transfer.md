---
title: 'call: transfer'
description: Переводить активный одноранговой звонок.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7c23ea17f1bc68b88490d8a54a68e50fe0604a78
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719778"
---
# <a name="call-transfer"></a><span data-ttu-id="4909e-103">call: transfer</span><span class="sxs-lookup"><span data-stu-id="4909e-103">call: transfer</span></span>

<span data-ttu-id="4909e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4909e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4909e-105">Переводить активный одноранговой звонок.</span><span class="sxs-lookup"><span data-stu-id="4909e-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="4909e-106">**Примечание.** Это поддерживается, только если и переносимый, и целевой объект переноса являются пользователями Microsoft Teams, принадлежащими одному и тем же арендатору.</span><span class="sxs-lookup"><span data-stu-id="4909e-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="4909e-107">Передача на номер STN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="4909e-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="4909e-108">Дополнительные информацию о переносимом, переносимом и целевом объекте см. в [RFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="4909e-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="4909e-109">Перенабор при консультации означает, что перед перенабором перед перенабором он может сообщить о перенаборе.</span><span class="sxs-lookup"><span data-stu-id="4909e-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="4909e-110">Это не касается прямой передачи вызова.</span><span class="sxs-lookup"><span data-stu-id="4909e-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="4909e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4909e-111">Permissions</span></span>
<span data-ttu-id="4909e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4909e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4909e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4909e-114">Permission type</span></span> | <span data-ttu-id="4909e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4909e-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="4909e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4909e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="4909e-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4909e-117">Not Supported</span></span>                |
| <span data-ttu-id="4909e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4909e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4909e-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4909e-119">Not Supported</span></span>                |
| <span data-ttu-id="4909e-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="4909e-120">Application</span></span>     | <span data-ttu-id="4909e-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="4909e-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="4909e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4909e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="4909e-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="4909e-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="4909e-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="4909e-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4909e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4909e-125">Request headers</span></span>
| <span data-ttu-id="4909e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="4909e-126">Name</span></span>          | <span data-ttu-id="4909e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4909e-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4909e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4909e-128">Authorization</span></span> | <span data-ttu-id="4909e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4909e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4909e-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4909e-131">Content-type</span></span>  | <span data-ttu-id="4909e-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4909e-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4909e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4909e-134">Request body</span></span>
<span data-ttu-id="4909e-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4909e-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4909e-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="4909e-136">Parameter</span></span>      | <span data-ttu-id="4909e-137">Тип</span><span class="sxs-lookup"><span data-stu-id="4909e-137">Type</span></span>    |<span data-ttu-id="4909e-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4909e-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4909e-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="4909e-139">transferTarget</span></span>|[<span data-ttu-id="4909e-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="4909e-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="4909e-141">Участник, который является целевым объектом передачи.</span><span class="sxs-lookup"><span data-stu-id="4909e-141">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="4909e-142">clientContext</span><span class="sxs-lookup"><span data-stu-id="4909e-142">clientContext</span></span>|<span data-ttu-id="4909e-143">String</span><span class="sxs-lookup"><span data-stu-id="4909e-143">String</span></span>|<span data-ttu-id="4909e-144">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="4909e-144">Unique Client Context string.</span></span> <span data-ttu-id="4909e-145">Максимальное ограничение — 256 chars.</span><span class="sxs-lookup"><span data-stu-id="4909e-145">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="4909e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4909e-146">Response</span></span>
<span data-ttu-id="4909e-147">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="4909e-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4909e-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="4909e-148">Examples</span></span>
<span data-ttu-id="4909e-149">В этих примерах показывается поток входящих вызовов в различных типах уведомлений о передаче.</span><span class="sxs-lookup"><span data-stu-id="4909e-149">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="4909e-150">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="4909e-150">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="4909e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="4909e-151">Request</span></span>
<span data-ttu-id="4909e-152">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4909e-152">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4909e-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="4909e-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4909e-154">C#</span><span class="sxs-lookup"><span data-stu-id="4909e-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4909e-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4909e-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4909e-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4909e-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4909e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="4909e-157">Response</span></span>

> <span data-ttu-id="4909e-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4909e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="4909e-160">Уведомление — передача</span><span class="sxs-lookup"><span data-stu-id="4909e-160">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="4909e-161">Уведомление — передача принимается</span><span class="sxs-lookup"><span data-stu-id="4909e-161">Notification - transfer accepted</span></span>

> <span data-ttu-id="4909e-162">**Примечание.** Передача, принятая, может происходить после или до нее неактивный звук состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4909e-162">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="4909e-163">Уведомление — передача завершена</span><span class="sxs-lookup"><span data-stu-id="4909e-163">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="4909e-164">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="4909e-164">Notification - transfer failed</span></span>

> <span data-ttu-id="4909e-165">**Примечание.** При сбойе перенаправки вызова состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="4909e-165">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="4909e-166">Пример 2. Передача консультаций</span><span class="sxs-lookup"><span data-stu-id="4909e-166">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="4909e-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="4909e-167">Request</span></span>
<span data-ttu-id="4909e-168">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4909e-168">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="4909e-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="4909e-169">Response</span></span>

> <span data-ttu-id="4909e-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4909e-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="4909e-172">Уведомление — передача</span><span class="sxs-lookup"><span data-stu-id="4909e-172">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="4909e-173">Уведомление — передача принимается</span><span class="sxs-lookup"><span data-stu-id="4909e-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="4909e-174">**Примечание.** Передача, принимаемая, может происходить после или до нее неактивный звук состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4909e-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="4909e-175">Уведомление — передача завершена</span><span class="sxs-lookup"><span data-stu-id="4909e-175">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="4909e-176">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="4909e-176">Notification - transfer failed</span></span>

> <span data-ttu-id="4909e-177">**Примечание.** При сбойе перенаправки вызова состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="4909e-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="4909e-178">Пример 3. Передача вызовов на номер STN</span><span class="sxs-lookup"><span data-stu-id="4909e-178">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="4909e-179">Для этого вызова требуется экземпляр приложения с назначенным номером STN.</span><span class="sxs-lookup"><span data-stu-id="4909e-179">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="4909e-180">Шаг 1. Создание экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="4909e-180">Step 1: Create application instance</span></span>
<span data-ttu-id="4909e-181">Используя учетные данные администратора клиента, вызовите следующие cmdlets в удаленной powerShell клиента, чтобы создать экземпляр приложения.</span><span class="sxs-lookup"><span data-stu-id="4909e-181">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="4909e-182">Дополнительные сведения см. в командах [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="4909e-182">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="4909e-183">Шаг 2. Назначение лицензий Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4909e-183">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="4909e-184">Используйте учетные данные администратора клиента для входа и перейдите на вкладку https://admin.microsoft.com/ **"Пользователи > активные пользователи".**</span><span class="sxs-lookup"><span data-stu-id="4909e-184">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="4909e-185">Выберите экземпляр приложения, назначьте план внутренних и международных звонков **Microsoft 365** и телефонную систему **Microsoft 365 —** лицензии виртуальных пользователей и нажмите кнопку **"Сохранить изменения".**</span><span class="sxs-lookup"><span data-stu-id="4909e-185">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="4909e-186">Если необходимые лицензии недоступны в клиенте, их можно получить на вкладке "Выставление счета **-> Приобретение служб".**</span><span class="sxs-lookup"><span data-stu-id="4909e-186">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="4909e-187">Шаг 3. Получение номера STN</span><span class="sxs-lookup"><span data-stu-id="4909e-187">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="4909e-188">Используйте учетные данные администратора клиента для входа и перейдите на вкладку "Устаревший https://admin.teams.microsoft.com/ **портал"** на левой панели.</span><span class="sxs-lookup"><span data-stu-id="4909e-188">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="4909e-189">На новой странице перейдите на вкладку **голосовых > номеров** телефонов.</span><span class="sxs-lookup"><span data-stu-id="4909e-189">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="4909e-190">Нажмите **+** кнопку, выберите **"Новые номера служб"** и перейдите на страницу **"Добавление новых номеров служб".**</span><span class="sxs-lookup"><span data-stu-id="4909e-190">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="4909e-191">Выберите **"Страна/регион",** **"Область",** **"Город",**"Количество **входных** данных" и нажмите **кнопку "Добавить"** для поиска.</span><span class="sxs-lookup"><span data-stu-id="4909e-191">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="4909e-192">Щелкните **"Получить номера".**</span><span class="sxs-lookup"><span data-stu-id="4909e-192">Click **acquire numbers**.</span></span> <span data-ttu-id="4909e-193">Недавно полученный номер будет показываться на **вкладке "Номера** телефонов".</span><span class="sxs-lookup"><span data-stu-id="4909e-193">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="4909e-194">Шаг 4. Назначение номера STN экземпляру приложения</span><span class="sxs-lookup"><span data-stu-id="4909e-194">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="4909e-195">С помощью учетных данных администратора клиента вызовите следующие cmdlets в удаленной powerShell клиента, чтобы назначить номер STN экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="4909e-195">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="4909e-196">Дополнительные сведения см. в командах [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="4909e-196">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
> <span data-ttu-id="4909e-197">**Примечание.** Если клиент имеет номера STN в Австралии, присвоенные экземплярам приложений, этот вызов может привести к сбойу.</span><span class="sxs-lookup"><span data-stu-id="4909e-197">**Note:** If a tenant has Australian PSTN numbers assigned to any application instances, this call might fail.</span></span> <span data-ttu-id="4909e-198">Если клиент создан только что, может потребоваться несколько дней, чтобы эта функция была доступна.</span><span class="sxs-lookup"><span data-stu-id="4909e-198">If a tenant is newly created, it might take several days for this feature to be available.</span></span>

#### <a name="request"></a><span data-ttu-id="4909e-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="4909e-199">Request</span></span>
<span data-ttu-id="4909e-200">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4909e-200">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="4909e-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="4909e-201">Response</span></span>

> <span data-ttu-id="4909e-p115">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4909e-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="4909e-204">Уведомление — передача</span><span class="sxs-lookup"><span data-stu-id="4909e-204">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="4909e-205">Уведомление — передача принимается</span><span class="sxs-lookup"><span data-stu-id="4909e-205">Notification - transfer accepted</span></span>

> <span data-ttu-id="4909e-206">**Примечание.** Передача, принятая, может происходить после или до нее неактивный звук состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4909e-206">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="4909e-207">Уведомление — передача завершена</span><span class="sxs-lookup"><span data-stu-id="4909e-207">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="4909e-208">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="4909e-208">Notification - transfer failed</span></span>

> <span data-ttu-id="4909e-209">**Примечание.** При сбойе перенаправки вызова состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="4909e-209">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="4909e-210">Пример 4. Консультационная передача на номер STN</span><span class="sxs-lookup"><span data-stu-id="4909e-210">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="4909e-211">Для этого вызова требуется экземпляр приложения с назначенным номером STN, как описано в примере 3.</span><span class="sxs-lookup"><span data-stu-id="4909e-211">This call requires an application instance with PSTN number assigned, as described in Example 3.</span></span>

> <span data-ttu-id="4909e-212">**Примечание.** Этот вызов может привести к сбойу, если клиент имеет номера STN в Австралии, присвоенные экземплярам приложений.</span><span class="sxs-lookup"><span data-stu-id="4909e-212">**Note:** This call may fail if a tenant has Australian PSTN numbers assigned to any application instances.</span></span> <span data-ttu-id="4909e-213">Если клиент создан только что, может потребоваться несколько дней, чтобы эта функция была доступна.</span><span class="sxs-lookup"><span data-stu-id="4909e-213">If a tenant is newly created, it might take several days for this feature to be available.</span></span>


#### <a name="request"></a><span data-ttu-id="4909e-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="4909e-214">Request</span></span>
<span data-ttu-id="4909e-215">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4909e-215">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="4909e-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="4909e-216">Response</span></span>

> <span data-ttu-id="4909e-p117">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4909e-p117">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="4909e-219">Уведомление — передача</span><span class="sxs-lookup"><span data-stu-id="4909e-219">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="4909e-220">Уведомление — передача принимается</span><span class="sxs-lookup"><span data-stu-id="4909e-220">Notification - transfer accepted</span></span>

> <span data-ttu-id="4909e-221">**Примечание.** Передача, принятая, может происходить после или до нее неактивный звук состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4909e-221">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="4909e-222">Уведомление — передача завершена</span><span class="sxs-lookup"><span data-stu-id="4909e-222">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="4909e-223">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="4909e-223">Notification - transfer failed</span></span>

> <span data-ttu-id="4909e-224">**Примечание.** При сбойе перенаправки вызова состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="4909e-224">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


