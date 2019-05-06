---
title: 'участник: выкл.'
description: Отключение выключения определенного участника в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0b5eeb42079b4628cc5ba988055d7081bb92dee9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595995"
---
# <a name="participant-mute"></a><span data-ttu-id="22d00-103">участник: выкл.</span><span class="sxs-lookup"><span data-stu-id="22d00-103">participant: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d00-104">Отключение выключения определенного участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="22d00-104">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="22d00-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22d00-105">Permissions</span></span>
<span data-ttu-id="22d00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22d00-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22d00-108">Permission type</span></span> | <span data-ttu-id="22d00-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22d00-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="22d00-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22d00-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="22d00-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="22d00-111">Not Supported</span></span>        |
| <span data-ttu-id="22d00-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22d00-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22d00-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="22d00-113">Not Supported</span></span>        |
| <span data-ttu-id="22d00-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22d00-114">Application</span></span>     | <span data-ttu-id="22d00-115">Нет</span><span class="sxs-lookup"><span data-stu-id="22d00-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="22d00-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22d00-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="22d00-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22d00-117">Request headers</span></span>
| <span data-ttu-id="22d00-118">Имя</span><span class="sxs-lookup"><span data-stu-id="22d00-118">Name</span></span>          | <span data-ttu-id="22d00-119">Описание</span><span class="sxs-lookup"><span data-stu-id="22d00-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="22d00-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22d00-120">Authorization</span></span> | <span data-ttu-id="22d00-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d00-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22d00-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22d00-123">Request body</span></span>
<span data-ttu-id="22d00-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="22d00-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="22d00-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="22d00-125">Parameter</span></span>      | <span data-ttu-id="22d00-126">Тип</span><span class="sxs-lookup"><span data-stu-id="22d00-126">Type</span></span>    |<span data-ttu-id="22d00-127">Описание</span><span class="sxs-lookup"><span data-stu-id="22d00-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22d00-128">Контекст</span><span class="sxs-lookup"><span data-stu-id="22d00-128">clientContext</span></span>|<span data-ttu-id="22d00-129">String</span><span class="sxs-lookup"><span data-stu-id="22d00-129">String</span></span>|<span data-ttu-id="22d00-130">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="22d00-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="22d00-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d00-131">Response</span></span>
<span data-ttu-id="22d00-132">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22d00-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22d00-133">Пример</span><span class="sxs-lookup"><span data-stu-id="22d00-133">Example</span></span>
<span data-ttu-id="22d00-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="22d00-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="22d00-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="22d00-135">Request</span></span>
<span data-ttu-id="22d00-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22d00-136">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="22d00-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d00-137">Response</span></span>

> <span data-ttu-id="22d00-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22d00-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="22d00-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="22d00-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="22d00-141">Языках</span><span class="sxs-lookup"><span data-stu-id="22d00-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/participant-mute-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22d00-142">Язык</span><span class="sxs-lookup"><span data-stu-id="22d00-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/participant-mute-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example---mute-specific-participant"></a><span data-ttu-id="22d00-143">Пример: Специальный участник</span><span class="sxs-lookup"><span data-stu-id="22d00-143">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="22d00-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="22d00-144">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="22d00-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d00-145">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="22d00-146">Список уведомлений обновлен с отключенным участником</span><span class="sxs-lookup"><span data-stu-id="22d00-146">Notification - roster updated with participant muted</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "0698446E77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "123456W77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-mute.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/participant-mute.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
