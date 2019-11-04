---
title: Удаление Календарпермиссион
description: Удаление Календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: def57ef9dab0f4c1666ebd9b411d9e05c7a75858
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936813"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="2e166-103">Удаление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="2e166-103">Delete calendarPermission</span></span>

<span data-ttu-id="2e166-104">Удаление Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="2e166-104">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e166-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e166-105">Permissions</span></span>

<span data-ttu-id="2e166-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e166-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e166-108">Permission type</span></span>      | <span data-ttu-id="2e166-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e166-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e166-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e166-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e166-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e166-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2e166-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e166-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e166-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e166-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2e166-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e166-114">Application</span></span> | <span data-ttu-id="2e166-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e166-115">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="2e166-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e166-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
DELETE /groups/{id}/calendar/calendarPermissions/{id}
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e166-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e166-117">Request headers</span></span>

| <span data-ttu-id="2e166-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2e166-118">Name</span></span>          | <span data-ttu-id="2e166-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2e166-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2e166-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e166-120">Authorization</span></span> | <span data-ttu-id="2e166-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2e166-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e166-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e166-122">Request body</span></span>

<span data-ttu-id="2e166-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e166-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e166-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e166-124">Response</span></span>

<span data-ttu-id="2e166-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2e166-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e166-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e166-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e166-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e166-128">Request</span></span>

<span data-ttu-id="2e166-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e166-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```

### <a name="response"></a><span data-ttu-id="2e166-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e166-130">Response</span></span>

<span data-ttu-id="2e166-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2e166-131">The following is an example of the response.</span></span>

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