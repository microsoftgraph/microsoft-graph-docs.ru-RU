---
title: 'Call: Transfer'
description: Передача активного однорангового звонка.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7be036e05bd772d01a9235427daa26b8044ba17e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440747"
---
# <a name="call-transfer"></a><span data-ttu-id="5d17a-103">Call: Transfer</span><span class="sxs-lookup"><span data-stu-id="5d17a-103">call: transfer</span></span>

<span data-ttu-id="5d17a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5d17a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d17a-105">Передача активного однорангового звонка.</span><span class="sxs-lookup"><span data-stu-id="5d17a-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="5d17a-106">**Примечание:** Поддерживается только в том случае, если целевой объект для передачи и передачи представляет пользователей Microsoft Teams, относящихся к одному и тому же клиенту.</span><span class="sxs-lookup"><span data-stu-id="5d17a-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="5d17a-107">Передача на номер PSTN не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d17a-107">Transfer to PSTN number is not supported.</span></span> <span data-ttu-id="5d17a-108">Чтобы узнать больше о переводу, переводу и целевом объекте для передачи, ознакомьтесь со статьей [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="5d17a-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="5d17a-109">Консультативногоная передача означает, что получатель может уведомить человека, которому он хочет передать вызов (передается), перед переносом.</span><span class="sxs-lookup"><span data-stu-id="5d17a-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="5d17a-110">Это в противоположность передаче вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="5d17a-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d17a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d17a-111">Permissions</span></span>
<span data-ttu-id="5d17a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d17a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d17a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d17a-114">Permission type</span></span> | <span data-ttu-id="5d17a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d17a-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="5d17a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d17a-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d17a-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5d17a-117">Not Supported</span></span>                |
| <span data-ttu-id="5d17a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d17a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d17a-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5d17a-119">Not Supported</span></span>                |
| <span data-ttu-id="5d17a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d17a-120">Application</span></span>     | <span data-ttu-id="5d17a-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="5d17a-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="5d17a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d17a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="5d17a-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="5d17a-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="5d17a-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="5d17a-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d17a-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d17a-125">Request headers</span></span>
| <span data-ttu-id="5d17a-126">Имя</span><span class="sxs-lookup"><span data-stu-id="5d17a-126">Name</span></span>          | <span data-ttu-id="5d17a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5d17a-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5d17a-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d17a-128">Authorization</span></span> | <span data-ttu-id="5d17a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d17a-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d17a-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d17a-131">Content-type</span></span>  | <span data-ttu-id="5d17a-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d17a-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d17a-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d17a-134">Request body</span></span>
<span data-ttu-id="5d17a-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5d17a-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d17a-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="5d17a-136">Parameter</span></span>      | <span data-ttu-id="5d17a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="5d17a-137">Type</span></span>    |<span data-ttu-id="5d17a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="5d17a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d17a-139">трансфертаржет</span><span class="sxs-lookup"><span data-stu-id="5d17a-139">transferTarget</span></span>|[<span data-ttu-id="5d17a-140">инвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="5d17a-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="5d17a-141">Участник, который является целевым объектом передачи.</span><span class="sxs-lookup"><span data-stu-id="5d17a-141">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="5d17a-142">Контекст</span><span class="sxs-lookup"><span data-stu-id="5d17a-142">clientContext</span></span>|<span data-ttu-id="5d17a-143">String</span><span class="sxs-lookup"><span data-stu-id="5d17a-143">String</span></span>|<span data-ttu-id="5d17a-144">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="5d17a-144">Unique Client Context string.</span></span> <span data-ttu-id="5d17a-145">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="5d17a-145">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="5d17a-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d17a-146">Response</span></span>
<span data-ttu-id="5d17a-147">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="5d17a-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5d17a-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="5d17a-148">Examples</span></span>
<span data-ttu-id="5d17a-149">В этих примерах показан входящий вызов для различных типов уведомлений о передаче.</span><span class="sxs-lookup"><span data-stu-id="5d17a-149">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="5d17a-150">Пример 1: Передача звонка</span><span class="sxs-lookup"><span data-stu-id="5d17a-150">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="5d17a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d17a-151">Request</span></span>
<span data-ttu-id="5d17a-152">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d17a-152">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5d17a-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d17a-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5d17a-154">C#</span><span class="sxs-lookup"><span data-stu-id="5d17a-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d17a-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d17a-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d17a-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d17a-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5d17a-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d17a-157">Response</span></span>

> <span data-ttu-id="5d17a-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d17a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="5d17a-160">Передача уведомлений</span><span class="sxs-lookup"><span data-stu-id="5d17a-160">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="5d17a-161">Уведомление — передача принята</span><span class="sxs-lookup"><span data-stu-id="5d17a-161">Notification - transfer accepted</span></span>

> <span data-ttu-id="5d17a-162">**Примечание:** Передача принята может быть выполнена после или до неактивного звука состояния носителя.</span><span class="sxs-lookup"><span data-stu-id="5d17a-162">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="5d17a-163">Уведомление о передаче завершено</span><span class="sxs-lookup"><span data-stu-id="5d17a-163">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="5d17a-164">Уведомление о сбое передачи</span><span class="sxs-lookup"><span data-stu-id="5d17a-164">Notification - transfer failed</span></span>

> <span data-ttu-id="5d17a-165">**Примечание:** При сбое передачи вызова в качестве состояния вызова будет использоваться `established`.</span><span class="sxs-lookup"><span data-stu-id="5d17a-165">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="5d17a-166">Пример 2: Консультативного Transfer</span><span class="sxs-lookup"><span data-stu-id="5d17a-166">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="5d17a-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d17a-167">Request</span></span>
<span data-ttu-id="5d17a-168">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d17a-168">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="5d17a-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d17a-169">Response</span></span>

> <span data-ttu-id="5d17a-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d17a-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="5d17a-172">Передача уведомлений</span><span class="sxs-lookup"><span data-stu-id="5d17a-172">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="5d17a-173">Уведомление — передача принята</span><span class="sxs-lookup"><span data-stu-id="5d17a-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="5d17a-174">**Примечание:** Передача принята может быть выполнена после или до неактивного звука состояния носителя.</span><span class="sxs-lookup"><span data-stu-id="5d17a-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="5d17a-175">Уведомление о передаче завершено</span><span class="sxs-lookup"><span data-stu-id="5d17a-175">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="5d17a-176">Уведомление о сбое передачи</span><span class="sxs-lookup"><span data-stu-id="5d17a-176">Notification - transfer failed</span></span>

> <span data-ttu-id="5d17a-177">**Примечание:** При сбое передачи вызова в качестве состояния вызова будет использоваться `established`.</span><span class="sxs-lookup"><span data-stu-id="5d17a-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
