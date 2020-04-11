---
title: Удаление Календарпермиссион
description: Удаление Календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 53e6c0cdf4edd1ad492f190bab488ba63d967219
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227925"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="94dc1-103">Удаление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="94dc1-103">Delete calendarPermission</span></span>

<span data-ttu-id="94dc1-104">Удаление Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="94dc1-104">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="94dc1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94dc1-105">Permissions</span></span>

<span data-ttu-id="94dc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94dc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94dc1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94dc1-108">Permission type</span></span>      | <span data-ttu-id="94dc1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94dc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94dc1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94dc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94dc1-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94dc1-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="94dc1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94dc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94dc1-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94dc1-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="94dc1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94dc1-114">Application</span></span> | <span data-ttu-id="94dc1-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94dc1-115">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="94dc1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94dc1-116">HTTP request</span></span>

<span data-ttu-id="94dc1-117">Удаление указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="94dc1-117">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="94dc1-118">Удаление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="94dc1-118">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="94dc1-119">Удаление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="94dc1-119">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94dc1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94dc1-120">Request headers</span></span>

| <span data-ttu-id="94dc1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="94dc1-121">Name</span></span>          | <span data-ttu-id="94dc1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="94dc1-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="94dc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94dc1-123">Authorization</span></span> | <span data-ttu-id="94dc1-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="94dc1-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="94dc1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94dc1-125">Request body</span></span>

<span data-ttu-id="94dc1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94dc1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94dc1-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="94dc1-127">Response</span></span>

<span data-ttu-id="94dc1-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="94dc1-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94dc1-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="94dc1-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94dc1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="94dc1-131">Request</span></span>

<span data-ttu-id="94dc1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94dc1-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/{id}
```

### <a name="response"></a><span data-ttu-id="94dc1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="94dc1-133">Response</span></span>

<span data-ttu-id="94dc1-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94dc1-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
