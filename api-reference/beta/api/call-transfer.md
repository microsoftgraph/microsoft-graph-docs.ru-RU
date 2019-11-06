---
title: 'Call: Transfer'
description: Передача активного однорангового звонка.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 14c2e1abae0dcc7729bfd7aa89a7a668555e60e8
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005901"
---
# <a name="call-transfer"></a><span data-ttu-id="2d3f8-103">Call: Transfer</span><span class="sxs-lookup"><span data-stu-id="2d3f8-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d3f8-104">Передача активного однорангового звонка.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-104">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="2d3f8-105">**Примечание:** Поддерживается только в том случае, если целевой объект для передачи и передачи представляет пользователей Microsoft Teams, относящихся к одному и тому же клиенту.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-105">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="2d3f8-106">Передача на номер PSTN не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-106">Transfer to PSTN number is not supported.</span></span> <span data-ttu-id="2d3f8-107">Чтобы узнать больше о переводу, переводу и целевом объекте для передачи, ознакомьтесь со статьей [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="2d3f8-107">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="2d3f8-108">Консультативногоная передача означает, что получатель может уведомить человека, которому он хочет передать вызов (передается), перед переносом.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-108">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="2d3f8-109">Это в противоположность передаче вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-109">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d3f8-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d3f8-110">Permissions</span></span>
<span data-ttu-id="2d3f8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d3f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d3f8-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d3f8-113">Permission type</span></span> | <span data-ttu-id="2d3f8-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d3f8-114">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="2d3f8-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d3f8-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d3f8-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2d3f8-116">Not Supported</span></span>                |
| <span data-ttu-id="2d3f8-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d3f8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d3f8-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2d3f8-118">Not Supported</span></span>                |
| <span data-ttu-id="2d3f8-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d3f8-119">Application</span></span>     | <span data-ttu-id="2d3f8-120">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="2d3f8-120">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="2d3f8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d3f8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="2d3f8-122">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-122">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="2d3f8-123">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-123">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d3f8-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d3f8-124">Request headers</span></span>
| <span data-ttu-id="2d3f8-125">Имя</span><span class="sxs-lookup"><span data-stu-id="2d3f8-125">Name</span></span>          | <span data-ttu-id="2d3f8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="2d3f8-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2d3f8-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d3f8-127">Authorization</span></span> | <span data-ttu-id="2d3f8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d3f8-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d3f8-130">Content-type</span></span>  | <span data-ttu-id="2d3f8-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d3f8-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d3f8-133">Request body</span></span>
<span data-ttu-id="2d3f8-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d3f8-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="2d3f8-135">Parameter</span></span>      | <span data-ttu-id="2d3f8-136">Тип</span><span class="sxs-lookup"><span data-stu-id="2d3f8-136">Type</span></span>    |<span data-ttu-id="2d3f8-137">Описание</span><span class="sxs-lookup"><span data-stu-id="2d3f8-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d3f8-138">трансфертаржет</span><span class="sxs-lookup"><span data-stu-id="2d3f8-138">transferTarget</span></span>|[<span data-ttu-id="2d3f8-139">инвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="2d3f8-139">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="2d3f8-140">Участник, который является целевым объектом передачи.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-140">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="2d3f8-141">Контекст</span><span class="sxs-lookup"><span data-stu-id="2d3f8-141">clientContext</span></span>|<span data-ttu-id="2d3f8-142">String</span><span class="sxs-lookup"><span data-stu-id="2d3f8-142">String</span></span>|<span data-ttu-id="2d3f8-143">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-143">Unique Client Context string.</span></span> <span data-ttu-id="2d3f8-144">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-144">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="2d3f8-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d3f8-145">Response</span></span>
<span data-ttu-id="2d3f8-146">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-146">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2d3f8-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d3f8-147">Examples</span></span>
<span data-ttu-id="2d3f8-148">В этих примерах показан входящий вызов для различных типов уведомлений о передаче.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-148">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="2d3f8-149">Пример 1: Передача звонка</span><span class="sxs-lookup"><span data-stu-id="2d3f8-149">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="2d3f8-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d3f8-150">Request</span></span>
<span data-ttu-id="2d3f8-151">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-151">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2d3f8-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d3f8-152">HTTP</span></span>](#tab/http)
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
    "region": "region-value",
    "replacesCallId": "replacesCallId-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d3f8-153">C#</span><span class="sxs-lookup"><span data-stu-id="2d3f8-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d3f8-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d3f8-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d3f8-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d3f8-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2d3f8-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d3f8-156">Response</span></span>

> <span data-ttu-id="2d3f8-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="2d3f8-159">Передача уведомлений</span><span class="sxs-lookup"><span data-stu-id="2d3f8-159">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="2d3f8-160">Уведомление — передача принята</span><span class="sxs-lookup"><span data-stu-id="2d3f8-160">Notification - transfer accepted</span></span>

> <span data-ttu-id="2d3f8-161">**Примечание:** Передача принята может быть выполнена после или до неактивного звука состояния носителя.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-161">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="2d3f8-162">Уведомление о передаче завершено</span><span class="sxs-lookup"><span data-stu-id="2d3f8-162">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="2d3f8-163">Уведомление о сбое передачи</span><span class="sxs-lookup"><span data-stu-id="2d3f8-163">Notification - transfer failed</span></span>

> <span data-ttu-id="2d3f8-164">**Примечание:** При сбое передачи вызова в качестве состояния вызова будет использоваться `established`.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-164">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="2d3f8-165">Пример 2: Консультативного Transfer</span><span class="sxs-lookup"><span data-stu-id="2d3f8-165">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="2d3f8-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d3f8-166">Request</span></span>
<span data-ttu-id="2d3f8-167">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-167">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="2d3f8-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d3f8-168">Response</span></span>

> <span data-ttu-id="2d3f8-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="2d3f8-171">Передача уведомлений</span><span class="sxs-lookup"><span data-stu-id="2d3f8-171">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="2d3f8-172">Уведомление — передача принята</span><span class="sxs-lookup"><span data-stu-id="2d3f8-172">Notification - transfer accepted</span></span>

> <span data-ttu-id="2d3f8-173">**Примечание:** Передача принята может быть выполнена после или до неактивного звука состояния носителя.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-173">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="2d3f8-174">Уведомление о передаче завершено</span><span class="sxs-lookup"><span data-stu-id="2d3f8-174">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="2d3f8-175">Уведомление о сбое передачи</span><span class="sxs-lookup"><span data-stu-id="2d3f8-175">Notification - transfer failed</span></span>

> <span data-ttu-id="2d3f8-176">**Примечание:** При сбое передачи вызова в качестве состояния вызова будет использоваться `established`.</span><span class="sxs-lookup"><span data-stu-id="2d3f8-176">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
