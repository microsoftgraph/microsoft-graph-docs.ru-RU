---
title: 'call: transfer'
description: Переводить активный одноранговой звонок.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 17597fd1dc7411da0d828af32feeba05433d5f2d
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238976"
---
# <a name="call-transfer"></a><span data-ttu-id="1c04b-103">call: transfer</span><span class="sxs-lookup"><span data-stu-id="1c04b-103">call: transfer</span></span>

<span data-ttu-id="1c04b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c04b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c04b-105">Переводить активный одноранговой звонок.</span><span class="sxs-lookup"><span data-stu-id="1c04b-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="1c04b-106">**Примечание.** Это поддерживается, только если и переносимый, и целевой объект передачи являются пользователями Microsoft Teams, принадлежащими одному и тем же арендатору.</span><span class="sxs-lookup"><span data-stu-id="1c04b-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="1c04b-107">Передача на номер STN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="1c04b-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="1c04b-108">Дополнительные информацию о переносимом, переносимом и целевом объекте см. в [RFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="1c04b-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="1c04b-109">Перенабор при консультации означает, что перед перенабором перед перенабором он может сообщить о перенаборе.</span><span class="sxs-lookup"><span data-stu-id="1c04b-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="1c04b-110">Это не касается прямой передачи вызова.</span><span class="sxs-lookup"><span data-stu-id="1c04b-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c04b-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c04b-111">Permissions</span></span>
<span data-ttu-id="1c04b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c04b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c04b-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c04b-114">Permission type</span></span> | <span data-ttu-id="1c04b-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c04b-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="1c04b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c04b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c04b-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1c04b-117">Not Supported</span></span>                |
| <span data-ttu-id="1c04b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c04b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c04b-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1c04b-119">Not Supported</span></span>                |
| <span data-ttu-id="1c04b-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c04b-120">Application</span></span>     | <span data-ttu-id="1c04b-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="1c04b-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="1c04b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c04b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="1c04b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c04b-123">Request headers</span></span>
| <span data-ttu-id="1c04b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1c04b-124">Name</span></span>          | <span data-ttu-id="1c04b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1c04b-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1c04b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c04b-126">Authorization</span></span> | <span data-ttu-id="1c04b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c04b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c04b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c04b-129">Content-type</span></span>  | <span data-ttu-id="1c04b-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c04b-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c04b-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c04b-132">Request body</span></span>
<span data-ttu-id="1c04b-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1c04b-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c04b-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="1c04b-134">Parameter</span></span>      | <span data-ttu-id="1c04b-135">Тип</span><span class="sxs-lookup"><span data-stu-id="1c04b-135">Type</span></span>    |<span data-ttu-id="1c04b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="1c04b-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c04b-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="1c04b-137">transferTarget</span></span>|[<span data-ttu-id="1c04b-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="1c04b-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="1c04b-139">Участник, который является целевым объектом передачи.</span><span class="sxs-lookup"><span data-stu-id="1c04b-139">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="1c04b-140">clientContext</span><span class="sxs-lookup"><span data-stu-id="1c04b-140">clientContext</span></span>|<span data-ttu-id="1c04b-141">String</span><span class="sxs-lookup"><span data-stu-id="1c04b-141">String</span></span>|<span data-ttu-id="1c04b-142">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="1c04b-142">Unique Client Context string.</span></span> <span data-ttu-id="1c04b-143">Максимальное ограничение — 256 chars.</span><span class="sxs-lookup"><span data-stu-id="1c04b-143">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="1c04b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c04b-144">Response</span></span>
<span data-ttu-id="1c04b-145">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="1c04b-145">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1c04b-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="1c04b-146">Examples</span></span>
<span data-ttu-id="1c04b-147">В этих примерах показывается поток входящих вызовов в различных типах уведомлений о передаче.</span><span class="sxs-lookup"><span data-stu-id="1c04b-147">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="1c04b-148">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="1c04b-148">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="1c04b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c04b-149">Request</span></span>
<span data-ttu-id="1c04b-150">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c04b-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c04b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c04b-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1c04b-152">C#</span><span class="sxs-lookup"><span data-stu-id="1c04b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c04b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c04b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c04b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c04b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c04b-155">Java</span><span class="sxs-lookup"><span data-stu-id="1c04b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1c04b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c04b-156">Response</span></span>

> <span data-ttu-id="1c04b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c04b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="1c04b-159">Уведомление — передача</span><span class="sxs-lookup"><span data-stu-id="1c04b-159">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="1c04b-160">Уведомление — передача принимается</span><span class="sxs-lookup"><span data-stu-id="1c04b-160">Notification - transfer accepted</span></span>

> <span data-ttu-id="1c04b-161">**Примечание.** Передача, принятая, может происходить после или до нее неактивный звук состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="1c04b-161">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="1c04b-162">Уведомление — передача завершена</span><span class="sxs-lookup"><span data-stu-id="1c04b-162">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="1c04b-163">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="1c04b-163">Notification - transfer failed</span></span>

> <span data-ttu-id="1c04b-164">**Примечание.** Если перенаправка звонка не удаться, состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="1c04b-164">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="1c04b-165">Пример 2. Передача консультаций</span><span class="sxs-lookup"><span data-stu-id="1c04b-165">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="1c04b-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c04b-166">Request</span></span>
<span data-ttu-id="1c04b-167">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c04b-167">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="1c04b-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c04b-168">Response</span></span>

> <span data-ttu-id="1c04b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c04b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="1c04b-171">Уведомление — передача</span><span class="sxs-lookup"><span data-stu-id="1c04b-171">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="1c04b-172">Уведомление — передача принимается</span><span class="sxs-lookup"><span data-stu-id="1c04b-172">Notification - transfer accepted</span></span>

> <span data-ttu-id="1c04b-173">**Примечание.** Передача, принятая, может происходить после или до нее неактивный звук состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="1c04b-173">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="1c04b-174">Уведомление — передача завершена</span><span class="sxs-lookup"><span data-stu-id="1c04b-174">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="1c04b-175">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="1c04b-175">Notification - transfer failed</span></span>

> <span data-ttu-id="1c04b-176">**Примечание.** Если перенаправка звонка не удаться, состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="1c04b-176">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="1c04b-177">Пример 3. Передача вызовов на номер STN</span><span class="sxs-lookup"><span data-stu-id="1c04b-177">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="1c04b-178">Для этого вызова требуется экземпляр приложения с назначенным номером STN.</span><span class="sxs-lookup"><span data-stu-id="1c04b-178">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="1c04b-179">Шаг 1. Создание экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="1c04b-179">Step 1: Create application instance</span></span>
<span data-ttu-id="1c04b-180">Используя учетные данные администратора клиента, вызовите следующие cmdlets в удаленной powerShell клиента, чтобы создать экземпляр приложения.</span><span class="sxs-lookup"><span data-stu-id="1c04b-180">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="1c04b-181">Дополнительные сведения см. в командах [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="1c04b-181">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="1c04b-182">Шаг 2. Назначение лицензий Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1c04b-182">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="1c04b-183">Используйте учетные данные администратора клиента для входа и перейдите на вкладку https://admin.microsoft.com/ **"Пользователи > активные пользователи".**</span><span class="sxs-lookup"><span data-stu-id="1c04b-183">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="1c04b-184">Выберите экземпляр приложения, назначьте план внутренних и международных звонков **Microsoft 365** и телефонную систему **Microsoft 365 —** лицензии виртуальных пользователей и нажмите кнопку **"Сохранить изменения".**</span><span class="sxs-lookup"><span data-stu-id="1c04b-184">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="1c04b-185">Если необходимые лицензии недоступны в клиенте, их можно получить на вкладке "Выставление счета **-> Приобретение служб".**</span><span class="sxs-lookup"><span data-stu-id="1c04b-185">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="1c04b-186">Шаг 3. Получение номера STN</span><span class="sxs-lookup"><span data-stu-id="1c04b-186">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="1c04b-187">Используйте учетные данные администратора клиента, чтобы войти в учетную панель и щелкнуть вкладку "Устаревший https://admin.teams.microsoft.com/ **портал"** на левой панели.</span><span class="sxs-lookup"><span data-stu-id="1c04b-187">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="1c04b-188">На новой странице перейдите на вкладку **голосовых > номеров** телефонов.</span><span class="sxs-lookup"><span data-stu-id="1c04b-188">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="1c04b-189">Нажмите **+** кнопку, выберите **"Новые номера служб"** и перейдите на страницу **"Добавление новых номеров служб".**</span><span class="sxs-lookup"><span data-stu-id="1c04b-189">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="1c04b-190">Выберите **"Страна/регион",** **"Область",** **"Город",**"Количество **входных** данных" и нажмите **кнопку "Добавить"** для поиска.</span><span class="sxs-lookup"><span data-stu-id="1c04b-190">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="1c04b-191">Щелкните **"Получить номера".**</span><span class="sxs-lookup"><span data-stu-id="1c04b-191">Click **acquire numbers**.</span></span> <span data-ttu-id="1c04b-192">Недавно полученный номер будет показываться на **вкладке "Номера** телефонов".</span><span class="sxs-lookup"><span data-stu-id="1c04b-192">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="1c04b-193">Шаг 4. Назначение номера STN экземпляру приложения</span><span class="sxs-lookup"><span data-stu-id="1c04b-193">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="1c04b-194">С помощью учетных данных администратора клиента вызовите следующие cmdlets в удаленной powerShell клиента, чтобы назначить номер STN экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="1c04b-194">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="1c04b-195">Дополнительные сведения см. в командах [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="1c04b-195">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```

#### <a name="request"></a><span data-ttu-id="1c04b-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c04b-196">Request</span></span>
<span data-ttu-id="1c04b-197">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c04b-197">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="1c04b-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c04b-198">Response</span></span>

> <span data-ttu-id="1c04b-p113">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c04b-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="1c04b-201">Уведомление — передача</span><span class="sxs-lookup"><span data-stu-id="1c04b-201">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="1c04b-202">Уведомление — передача принимается</span><span class="sxs-lookup"><span data-stu-id="1c04b-202">Notification - transfer accepted</span></span>

> <span data-ttu-id="1c04b-203">**Примечание.** Передача, принятая, может происходить после или до нее неактивный звук состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="1c04b-203">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="1c04b-204">Уведомление — передача завершена</span><span class="sxs-lookup"><span data-stu-id="1c04b-204">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="1c04b-205">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="1c04b-205">Notification - transfer failed</span></span>

> <span data-ttu-id="1c04b-206">**Примечание.** Если перенаправка звонка не удаться, состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="1c04b-206">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="1c04b-207">Пример 4. Консультационная передача на номер STN</span><span class="sxs-lookup"><span data-stu-id="1c04b-207">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="1c04b-208">Для этого вызова требуется экземпляр приложения с назначенным номером STN, как описано в примере 3.</span><span class="sxs-lookup"><span data-stu-id="1c04b-208">This call requires an application instance with PSTN number assigned, as described in Example 3.</span></span>

#### <a name="request"></a><span data-ttu-id="1c04b-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c04b-209">Request</span></span>
<span data-ttu-id="1c04b-210">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c04b-210">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="1c04b-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c04b-211">Response</span></span>

> <span data-ttu-id="1c04b-p114">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c04b-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="1c04b-214">Уведомление — передача</span><span class="sxs-lookup"><span data-stu-id="1c04b-214">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="1c04b-215">Уведомление — передача принимается</span><span class="sxs-lookup"><span data-stu-id="1c04b-215">Notification - transfer accepted</span></span>

> <span data-ttu-id="1c04b-216">**Примечание.** Передача, принятая, может происходить после или до нее неактивный звук состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="1c04b-216">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="1c04b-217">Уведомление — передача завершена</span><span class="sxs-lookup"><span data-stu-id="1c04b-217">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="1c04b-218">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="1c04b-218">Notification - transfer failed</span></span>

> <span data-ttu-id="1c04b-219">**Примечание.** Если перенаправка звонка не удаться, состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="1c04b-219">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

