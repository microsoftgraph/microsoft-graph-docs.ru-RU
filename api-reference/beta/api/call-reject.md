---
title: 'Вызовите: отклонить'
description: Отклонение входящего звонка.
author: VinodRavichandran
ms.openlocfilehash: 2516ead8d9fa158192a0d9c7c02ac8adb44f764a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343458"
---
# <a name="call-reject"></a><span data-ttu-id="59e50-103">Вызовите: отклонить</span><span class="sxs-lookup"><span data-stu-id="59e50-103">call: reject</span></span>

> <span data-ttu-id="59e50-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="59e50-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59e50-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59e50-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59e50-106">Отклонение входящего звонка.</span><span class="sxs-lookup"><span data-stu-id="59e50-106">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="59e50-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59e50-107">Permissions</span></span>
<span data-ttu-id="59e50-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59e50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59e50-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59e50-110">Permission type</span></span> | <span data-ttu-id="59e50-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59e50-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="59e50-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59e50-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="59e50-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="59e50-113">Not Supported</span></span>                       |
| <span data-ttu-id="59e50-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59e50-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59e50-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="59e50-115">Not Supported</span></span>                       |
| <span data-ttu-id="59e50-116">Application</span><span class="sxs-lookup"><span data-stu-id="59e50-116">Application</span></span>     | <span data-ttu-id="59e50-117">Нет</span><span class="sxs-lookup"><span data-stu-id="59e50-117">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="59e50-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59e50-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="59e50-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59e50-119">Request headers</span></span>
| <span data-ttu-id="59e50-120">Имя</span><span class="sxs-lookup"><span data-stu-id="59e50-120">Name</span></span>          | <span data-ttu-id="59e50-121">Описание</span><span class="sxs-lookup"><span data-stu-id="59e50-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="59e50-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59e50-122">Authorization</span></span> | <span data-ttu-id="59e50-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59e50-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59e50-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59e50-125">Request body</span></span>
<span data-ttu-id="59e50-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="59e50-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59e50-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="59e50-127">Parameter</span></span>      | <span data-ttu-id="59e50-128">Тип</span><span class="sxs-lookup"><span data-stu-id="59e50-128">Type</span></span>    |<span data-ttu-id="59e50-129">Описание</span><span class="sxs-lookup"><span data-stu-id="59e50-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59e50-130">Причина</span><span class="sxs-lookup"><span data-stu-id="59e50-130">reason</span></span>|<span data-ttu-id="59e50-131">String.</span><span class="sxs-lookup"><span data-stu-id="59e50-131">String</span></span>|<span data-ttu-id="59e50-132">Причину отклонения.</span><span class="sxs-lookup"><span data-stu-id="59e50-132">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="59e50-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="59e50-133">Response</span></span>
<span data-ttu-id="59e50-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="59e50-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="59e50-136">Пример</span><span class="sxs-lookup"><span data-stu-id="59e50-136">Example</span></span>
<span data-ttu-id="59e50-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="59e50-137">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="59e50-138">Уведомления - входящие</span><span class="sxs-lookup"><span data-stu-id="59e50-138">Notification - incoming</span></span>

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
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="59e50-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="59e50-139">Request</span></span>
<span data-ttu-id="59e50-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59e50-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```

##### <a name="response"></a><span data-ttu-id="59e50-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="59e50-141">Response</span></span>
<span data-ttu-id="59e50-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="59e50-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="59e50-143">Уведомления - удалены</span><span class="sxs-lookup"><span data-stu-id="59e50-143">Notification - deleted</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\""
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
