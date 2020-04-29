---
title: Создание или замена действия
description: Создание нового или замена существующего действия пользователя для вашего приложения. Если вы хотите создать действия пользователя и связанные с ним **historyitem** в одном запросе, вы можете использовать глубокую вставку.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: 7ca7d0d5b222c7e82a9dbd108071174a0df09d23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510720"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="ed262-104">Создание или замена действия</span><span class="sxs-lookup"><span data-stu-id="ed262-104">Create or replace an activity</span></span>

<span data-ttu-id="ed262-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed262-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed262-106">Создание нового или замена существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="ed262-106">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="ed262-107">Если вы хотите создать действия пользователя и связанные с ним **historyitem** в одном запросе, вы можете использовать [глубокую вставку](#example-2-deep-insert).</span><span class="sxs-lookup"><span data-stu-id="ed262-107">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](#example-2-deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed262-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed262-108">Permissions</span></span>

<span data-ttu-id="ed262-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed262-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed262-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed262-111">Permission type</span></span>                        | <span data-ttu-id="ed262-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed262-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="ed262-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed262-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed262-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ed262-114">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="ed262-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed262-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed262-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ed262-116">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="ed262-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed262-117">Application</span></span>                            | <span data-ttu-id="ed262-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed262-118">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="ed262-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed262-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

> <span data-ttu-id="ed262-120">**Примечание:** Аппактивитид в URL-адресе должен быть безопасным по URL-адресу (все символы, кроме зарезервированных символов RFC 2396, должны быть преобразованы в шестнадцатеричное представление), но исходный Аппактивитид не обязательно должен быть безопасным по URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="ed262-120">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed262-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed262-121">Request headers</span></span>

| <span data-ttu-id="ed262-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ed262-122">Name</span></span>          | <span data-ttu-id="ed262-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ed262-123">Type</span></span>   | <span data-ttu-id="ed262-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ed262-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="ed262-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed262-125">Authorization</span></span> | <span data-ttu-id="ed262-126">string</span><span class="sxs-lookup"><span data-stu-id="ed262-126">string</span></span> | <span data-ttu-id="ed262-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed262-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed262-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed262-129">Request body</span></span>

<span data-ttu-id="ed262-130">В тексте запроса добавьте представление объекта [Activity](../resources/projectrome-activity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed262-130">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ed262-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed262-131">Response</span></span>

<span data-ttu-id="ed262-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, если действие было `200 OK` создано, или если действие было заменено.</span><span class="sxs-lookup"><span data-stu-id="ed262-132">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="examples"></a><span data-ttu-id="ed262-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="ed262-133">Examples</span></span>

### <a name="example-1-create-an-activity"></a><span data-ttu-id="ed262-134">Пример 1: Создание действия</span><span class="sxs-lookup"><span data-stu-id="ed262-134">Example 1: Create an activity</span></span>

#### <a name="request"></a><span data-ttu-id="ed262-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed262-135">Request</span></span>

<span data-ttu-id="ed262-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed262-136">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

{
  "appActivityId": "/article?12345",
  "activitySourceHost": "https://www.contoso.com",
  "userTimezone": "Africa/Casablanca",
  "appDisplayName": "Contoso, Ltd.",
  "activationUrl": "https://www.contoso.com/article?id=12345",
  "contentUrl": "https://www.contoso.com/article?id=12345",
  "fallbackUrl": "https://www.contoso.com/article?id=12345",
  "contentInfo": {
    "@context": "https://schema.org",
    "@type": "Article",
    "author": "Jennifer Booth",
    "name": "How to Tie a Reef Knot"
  },
  "visualElements": {
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": false
    },
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "backgroundColor": "#ff0000",
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="ed262-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed262-137">Response</span></span>

<span data-ttu-id="ed262-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed262-138">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  },
  "activationUrl": "https://www.contoso.com/article?id=12345",
  "appDisplayName": "Contoso, Ltd.",
  "userTimezone": "Africa/Casablanca",
  "fallbackUrl": "https://www.contoso.com/article?id=12345",
  "contentUrl": "https://www.contoso.com/article?id=12345",
  "contentInfo": {
    "@context": "https://schema.org",
    "@type": "Article",
    "author": "Jennifer Booth",
    "name": "How to Tie a Reef Knot"
  }
}
```

### <a name="example-2-deep-insert"></a><span data-ttu-id="ed262-139">Пример 2: глубокая Вставка</span><span class="sxs-lookup"><span data-stu-id="ed262-139">Example 2: Deep insert</span></span>

<span data-ttu-id="ed262-140">В этом примере показано создание нового действия и элемента журнала для этого действия в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="ed262-140">This example creates a new activity and a history item for that activity in one request.</span></span>

#### <a name="request"></a><span data-ttu-id="ed262-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed262-141">Request</span></span>

<span data-ttu-id="ed262-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed262-142">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

{
  "appActivityId": "/article?12345",
  "activitySourceHost": "https://www.contoso.com",
  "userTimezone": "Africa/Casablanca",
  "appDisplayName": "Contoso, Ltd.",
  "activationUrl": "https://www.contoso.com/article?id=12345",
  "contentUrl": "https://www.contoso.com/article?id=12345",
  "fallbackUrl": "https://www.contoso.com/article?id=12345",
  "contentInfo": {
    "@context": "https://schema.org",
    "@type": "Article",
    "author": "Jennifer Booth",
    "name": "How to Tie a Reef Knot"
  },
  "visualElements": {
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "backgroundColor": "#ff0000",
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  },
  "historyItems": [
    {
      "userTimezone": "Africa/Casablanca",
      "startedDateTime": "2018-02-26T20:54:04.345Z",
      "lastActiveDateTime": "2018-02-26T20:54:24.345Z"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="ed262-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed262-143">Response</span></span>

<span data-ttu-id="ed262-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ed262-144">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  },
  "activationUrl": "https://www.contoso.com/article?id=12345",
  "appDisplayName": "Contoso, Ltd.",
  "userTimezone": "Africa/Casablanca",
  "fallbackUrl": "https://www.contoso.com/article?id=12345",
  "contentUrl": "https://www.contoso.com/article?id=12345",
  "contentInfo": {
    "@context": "https://schema.org",
    "@type": "Article",
    "author": "Jennifer Booth",
    "name": "How to Tie a Reef Knot"
  },
  "historyItems": [
    {
      "status": "updated",
      "userTimezone": "Africa/Casablanca",
      "createdDateTime": "2018-04-12T21:42:42.495Z",
      "lastModifiedDateTime": "2018-04-12T21:42:42.495Z",
      "id": "61fc8f36-919f-4b73-89d4-1cb7b159d912",
      "startedDateTime": "2018-02-26T20:54:04.345Z",
      "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
      "expirationDateTime": "2018-05-12T21:42:42.495Z",
      "activeDurationSeconds": 20
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
