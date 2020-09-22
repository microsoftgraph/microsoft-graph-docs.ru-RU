---
title: Создание или замена объекта historyItem
description: Создание нового или замена существующего элемента журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: ee46c25555e3621bd18d020bd3312bd7b1d543aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083311"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="e5a87-103">Создание или замена объекта historyItem</span><span class="sxs-lookup"><span data-stu-id="e5a87-103">Create or replace a historyItem</span></span>

<span data-ttu-id="e5a87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5a87-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5a87-105">Создание нового или замена существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="e5a87-105">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5a87-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5a87-106">Permissions</span></span>

<span data-ttu-id="e5a87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5a87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e5a87-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5a87-109">Permission type</span></span>      | <span data-ttu-id="e5a87-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5a87-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5a87-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5a87-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e5a87-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e5a87-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e5a87-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5a87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5a87-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e5a87-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e5a87-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5a87-115">Application</span></span> | <span data-ttu-id="e5a87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5a87-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5a87-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5a87-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="e5a87-118">Идентификатор должен быть идентификатором GUID.</span><span class="sxs-lookup"><span data-stu-id="e5a87-118">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5a87-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5a87-119">Request headers</span></span>

|<span data-ttu-id="e5a87-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e5a87-120">Name</span></span> | <span data-ttu-id="e5a87-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e5a87-121">Type</span></span> | <span data-ttu-id="e5a87-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e5a87-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="e5a87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5a87-123">Authorization</span></span> | <span data-ttu-id="e5a87-124">string</span><span class="sxs-lookup"><span data-stu-id="e5a87-124">string</span></span> | <span data-ttu-id="e5a87-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5a87-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5a87-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5a87-127">Request body</span></span>

<span data-ttu-id="e5a87-128">В тексте запроса добавьте представление объекта [historyItem](../resources/projectrome-historyitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5a87-128">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e5a87-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5a87-129">Response</span></span>

<span data-ttu-id="e5a87-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, если был создан historyItem, или `200 OK` Если historyItem был заменен.</span><span class="sxs-lookup"><span data-stu-id="e5a87-130">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="e5a87-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e5a87-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e5a87-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5a87-132">Request</span></span>

<span data-ttu-id="e5a87-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5a87-133">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="e5a87-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5a87-134">Response</span></span>

<span data-ttu-id="e5a87-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5a87-135">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activityHistoryItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
    "status": "updated",
    "userTimezone": "Africa/Casablanca",
    "createdDateTime": "2018-02-26T20:28:22.14Z",
    "lastModifiedDateTime": "2018-02-26T20:28:22.155Z",
    "id": "9d0b74e4-4b41-43ea-b34d-f9c1bf9f809c",
    "startedDateTime": "2018-02-26T20:54:04.345Z",
    "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
    "expirationDateTime": "2018-03-28T20:28:22.14Z",
    "activeDurationSeconds": 20
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

