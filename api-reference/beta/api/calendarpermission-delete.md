---
title: Удаление Календарпермиссион
description: Удаление Календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 13756f6a5c84b999b7322341b65030767535807c
ms.sourcegitcommit: 1a3ca53422fc9a8254e78af7c058e876fc9f9ef8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2019
ms.locfileid: "37942652"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="cf27b-103">Удаление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="cf27b-103">Delete calendarPermission</span></span>

<span data-ttu-id="cf27b-104">Удаление Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="cf27b-104">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf27b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf27b-105">Permissions</span></span>

<span data-ttu-id="cf27b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf27b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf27b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf27b-108">Permission type</span></span>      | <span data-ttu-id="cf27b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf27b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf27b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf27b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf27b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf27b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cf27b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf27b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf27b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf27b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cf27b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf27b-114">Application</span></span> | <span data-ttu-id="cf27b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf27b-115">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="cf27b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf27b-116">HTTP request</span></span>

<span data-ttu-id="cf27b-117">Удаление указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="cf27b-117">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="cf27b-118">Удаление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="cf27b-118">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="cf27b-119">Удаление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="cf27b-119">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cf27b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf27b-120">Request headers</span></span>

| <span data-ttu-id="cf27b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cf27b-121">Name</span></span>          | <span data-ttu-id="cf27b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cf27b-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cf27b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf27b-123">Authorization</span></span> | <span data-ttu-id="cf27b-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="cf27b-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf27b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf27b-125">Request body</span></span>

<span data-ttu-id="cf27b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf27b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf27b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf27b-127">Response</span></span>

<span data-ttu-id="cf27b-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cf27b-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf27b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="cf27b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf27b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf27b-131">Request</span></span>

<span data-ttu-id="cf27b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf27b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```

### <a name="response"></a><span data-ttu-id="cf27b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf27b-133">Response</span></span>

<span data-ttu-id="cf27b-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cf27b-134">The following is an example of the response.</span></span>

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