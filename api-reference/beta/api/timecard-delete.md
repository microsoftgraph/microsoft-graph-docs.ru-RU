---
title: Удаление timeCard
description: Удаление экземпляра timeCard в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f87fe8145d65793b33dc539ed1db235a7e09aebf
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787919"
---
# <a name="delete-timecard"></a><span data-ttu-id="4f71b-103">Удаление timeCard</span><span class="sxs-lookup"><span data-stu-id="4f71b-103">Delete timeCard</span></span>

<span data-ttu-id="4f71b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f71b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f71b-105">Удаление [экземпляра timeCard](../resources/timeCard.md) в [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="4f71b-105">Delete a [timeCard](../resources/timeCard.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f71b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f71b-106">Permissions</span></span>

<span data-ttu-id="4f71b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f71b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f71b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f71b-109">Permission type</span></span>      | <span data-ttu-id="4f71b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f71b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f71b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f71b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f71b-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f71b-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f71b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f71b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f71b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f71b-114">Not supported.</span></span>    |
|<span data-ttu-id="4f71b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f71b-115">Application</span></span> | <span data-ttu-id="4f71b-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="4f71b-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="4f71b-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="4f71b-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="4f71b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f71b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="4f71b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f71b-119">Request headers</span></span>

| <span data-ttu-id="4f71b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f71b-120">Header</span></span>       | <span data-ttu-id="4f71b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4f71b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f71b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f71b-122">Authorization</span></span>  | <span data-ttu-id="4f71b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f71b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4f71b-125">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="4f71b-125">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="4f71b-126">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="4f71b-126">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="4f71b-127">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="4f71b-127">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f71b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f71b-128">Request body</span></span>
<span data-ttu-id="4f71b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f71b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f71b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f71b-130">Response</span></span>

<span data-ttu-id="4f71b-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4f71b-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4f71b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4f71b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f71b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f71b-133">Request</span></span>
<span data-ttu-id="4f71b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f71b-134">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-delete"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards/3895809b-a618-4c0d-86a0-d42b25b7d74f
```

### <a name="response"></a><span data-ttu-id="4f71b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f71b-135">Response</span></span>

<span data-ttu-id="4f71b-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4f71b-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
