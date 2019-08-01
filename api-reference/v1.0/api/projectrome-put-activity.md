---
title: Создание или замена действия
description: Создание нового или замена существующего действия пользователя для вашего приложения. Если вы хотите создать действия пользователя и связанные с ним **historyitem** в одном запросе, вы можете использовать глубокую вставку.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: 8f80d17f64b4f04816670d8e007ca7db82755c0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025374"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="5520f-104">Создание или замена действия</span><span class="sxs-lookup"><span data-stu-id="5520f-104">Create or replace an activity</span></span>

<span data-ttu-id="5520f-105">Создание нового или замена существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="5520f-105">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="5520f-106">Если вы хотите создать действия пользователя и связанные с ним **historyitem** в одном запросе, вы можете использовать глубокую [вставку](#example-2-deep-insert).</span><span class="sxs-lookup"><span data-stu-id="5520f-106">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](#example-2-deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="5520f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5520f-107">Permissions</span></span>

<span data-ttu-id="5520f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5520f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5520f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5520f-110">Permission type</span></span>                        | <span data-ttu-id="5520f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5520f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="5520f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5520f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5520f-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5520f-113">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="5520f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5520f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5520f-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5520f-115">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="5520f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5520f-116">Application</span></span>                            | <span data-ttu-id="5520f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5520f-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="5520f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5520f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

> <span data-ttu-id="5520f-119">**Примечание:** Аппактивитид в URL-адресе должен быть безопасным по URL-адресу (все символы, кроме зарезервированных символов RFC 2396, должны быть преобразованы в шестнадцатеричное представление), но исходный Аппактивитид не обязательно должен быть безопасным по URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="5520f-119">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5520f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5520f-120">Request headers</span></span>

| <span data-ttu-id="5520f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5520f-121">Name</span></span>          | <span data-ttu-id="5520f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5520f-122">Type</span></span>   | <span data-ttu-id="5520f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5520f-123">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="5520f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5520f-124">Authorization</span></span> | <span data-ttu-id="5520f-125">string</span><span class="sxs-lookup"><span data-stu-id="5520f-125">string</span></span> | <span data-ttu-id="5520f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5520f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5520f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5520f-128">Request body</span></span>

<span data-ttu-id="5520f-129">В тексте запроса добавьте представление объекта [Activity](../resources/projectrome-activity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5520f-129">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5520f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5520f-130">Response</span></span>

<span data-ttu-id="5520f-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, если действие было `200 OK` создано, или если действие было заменено.</span><span class="sxs-lookup"><span data-stu-id="5520f-131">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="examples"></a><span data-ttu-id="5520f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="5520f-132">Examples</span></span>

### <a name="example-1-create-an-activity"></a><span data-ttu-id="5520f-133">Пример 1: Создание действия</span><span class="sxs-lookup"><span data-stu-id="5520f-133">Example 1: Create an activity</span></span>

#### <a name="request"></a><span data-ttu-id="5520f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5520f-134">Request</span></span>

<span data-ttu-id="5520f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5520f-135">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="5520f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5520f-136">Response</span></span>

<span data-ttu-id="5520f-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5520f-137">The following is an example of the response.</span></span>

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

### <a name="example-2-deep-insert"></a><span data-ttu-id="5520f-138">Пример 2: глубокая Вставка</span><span class="sxs-lookup"><span data-stu-id="5520f-138">Example 2: Deep insert</span></span>

<span data-ttu-id="5520f-139">В этом примере показано создание нового действия и элемента журнала для этого действия в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="5520f-139">This example creates a new activity and a history item for that activity in one request.</span></span>

#### <a name="request"></a><span data-ttu-id="5520f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5520f-140">Request</span></span>

<span data-ttu-id="5520f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5520f-141">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="5520f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5520f-142">Response</span></span>

<span data-ttu-id="5520f-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5520f-143">The following is an example of the response.</span></span>

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
