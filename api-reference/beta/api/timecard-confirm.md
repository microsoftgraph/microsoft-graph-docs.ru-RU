---
title: 'timeCard: подтверждение'
description: Подтвердим определенную химкарь.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 42ee0d8c1259b31ebf96716ca1c49656af4075f8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787925"
---
# <a name="timecard-confirm"></a><span data-ttu-id="0f2fe-103">timeCard: подтверждение</span><span class="sxs-lookup"><span data-stu-id="0f2fe-103">timeCard: confirm</span></span>

<span data-ttu-id="0f2fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f2fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f2fe-105">Подтвердим [определенный timeCard](../resources/timeCard.md).</span><span class="sxs-lookup"><span data-stu-id="0f2fe-105">Confirm a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f2fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f2fe-106">Permissions</span></span>

<span data-ttu-id="0f2fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f2fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f2fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f2fe-109">Permission type</span></span>      | <span data-ttu-id="0f2fe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f2fe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f2fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f2fe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f2fe-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f2fe-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f2fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f2fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f2fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f2fe-114">Not supported.</span></span>    |
|<span data-ttu-id="0f2fe-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0f2fe-115">Application</span></span> | <span data-ttu-id="0f2fe-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="0f2fe-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="0f2fe-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="0f2fe-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="0f2fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f2fe-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/confirm
```

## <a name="request-headers"></a><span data-ttu-id="0f2fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f2fe-119">Request headers</span></span>

| <span data-ttu-id="0f2fe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f2fe-120">Header</span></span>       | <span data-ttu-id="0f2fe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0f2fe-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f2fe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f2fe-122">Authorization</span></span>  | <span data-ttu-id="0f2fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f2fe-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0f2fe-125">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="0f2fe-125">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="0f2fe-126">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="0f2fe-126">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="0f2fe-127">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="0f2fe-127">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f2fe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f2fe-128">Request body</span></span>
<span data-ttu-id="0f2fe-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f2fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f2fe-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f2fe-130">Response</span></span>

<span data-ttu-id="0f2fe-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0f2fe-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0f2fe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0f2fe-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f2fe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f2fe-133">Request</span></span>
<span data-ttu-id="0f2fe-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f2fe-134">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-confirm"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/confirm
```

### <a name="response"></a><span data-ttu-id="0f2fe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f2fe-135">Response</span></span>

<span data-ttu-id="0f2fe-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0f2fe-136">The following is an example of the response.</span></span> 

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
  "description": "Confirm timecard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
