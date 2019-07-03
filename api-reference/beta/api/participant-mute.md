---
title: 'участник: выкл.'
description: Отключение выключения определенного участника в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6dd848ae967f657bf4639418eee3d4e8815b546e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453945"
---
# <a name="participant-mute"></a><span data-ttu-id="b43ed-103">участник: выкл.</span><span class="sxs-lookup"><span data-stu-id="b43ed-103">participant: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b43ed-104">Отключение выключения определенного участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="b43ed-104">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="b43ed-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b43ed-105">Permissions</span></span>
<span data-ttu-id="b43ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b43ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b43ed-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b43ed-108">Permission type</span></span> | <span data-ttu-id="b43ed-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b43ed-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="b43ed-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b43ed-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b43ed-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b43ed-111">Not Supported</span></span>        |
| <span data-ttu-id="b43ed-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b43ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b43ed-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b43ed-113">Not Supported</span></span>        |
| <span data-ttu-id="b43ed-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b43ed-114">Application</span></span>     | <span data-ttu-id="b43ed-115">Нет</span><span class="sxs-lookup"><span data-stu-id="b43ed-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="b43ed-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b43ed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="b43ed-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b43ed-117">Request headers</span></span>
| <span data-ttu-id="b43ed-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b43ed-118">Name</span></span>          | <span data-ttu-id="b43ed-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b43ed-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b43ed-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b43ed-120">Authorization</span></span> | <span data-ttu-id="b43ed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b43ed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b43ed-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b43ed-123">Request body</span></span>
<span data-ttu-id="b43ed-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b43ed-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b43ed-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="b43ed-125">Parameter</span></span>      | <span data-ttu-id="b43ed-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b43ed-126">Type</span></span>    |<span data-ttu-id="b43ed-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b43ed-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b43ed-128">Контекст</span><span class="sxs-lookup"><span data-stu-id="b43ed-128">clientContext</span></span>|<span data-ttu-id="b43ed-129">String</span><span class="sxs-lookup"><span data-stu-id="b43ed-129">String</span></span>|<span data-ttu-id="b43ed-130">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="b43ed-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="b43ed-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b43ed-131">Response</span></span>
<span data-ttu-id="b43ed-132">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b43ed-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b43ed-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b43ed-133">Example</span></span>
<span data-ttu-id="b43ed-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b43ed-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b43ed-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b43ed-135">Request</span></span>
<span data-ttu-id="b43ed-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b43ed-136">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b43ed-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b43ed-137">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b43ed-138">C#</span><span class="sxs-lookup"><span data-stu-id="b43ed-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b43ed-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="b43ed-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b43ed-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b43ed-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b43ed-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b43ed-141">Response</span></span>

> <span data-ttu-id="b43ed-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b43ed-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="example---mute-specific-participant"></a><span data-ttu-id="b43ed-144">Пример: Специальный участник</span><span class="sxs-lookup"><span data-stu-id="b43ed-144">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="b43ed-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b43ed-145">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="b43ed-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b43ed-146">Response</span></span>

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

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="b43ed-147">Список уведомлений обновлен с отключенным участником</span><span class="sxs-lookup"><span data-stu-id="b43ed-147">Notification - roster updated with participant muted</span></span>

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
  ]
}
-->
