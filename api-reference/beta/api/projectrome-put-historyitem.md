---
title: Создание или замена объекта historyItem
description: Создание нового или замена существующего элемента журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 0a8d03029350ce96e7442473dffa0595278bc195
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337279"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="3ab70-103">Создание или замена объекта historyItem</span><span class="sxs-lookup"><span data-stu-id="3ab70-103">Create or replace a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ab70-104">Создание нового или замена существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="3ab70-104">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ab70-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ab70-105">Permissions</span></span>

<span data-ttu-id="3ab70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ab70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3ab70-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ab70-108">Permission type</span></span>      | <span data-ttu-id="3ab70-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ab70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ab70-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ab70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ab70-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="3ab70-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="3ab70-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ab70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ab70-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="3ab70-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="3ab70-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ab70-114">Application</span></span> | <span data-ttu-id="3ab70-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ab70-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ab70-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ab70-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="3ab70-117">Идентификатор должен быть ИДЕНТИФИКАТОРом GUID.</span><span class="sxs-lookup"><span data-stu-id="3ab70-117">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ab70-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ab70-118">Request headers</span></span>

|<span data-ttu-id="3ab70-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3ab70-119">Name</span></span> | <span data-ttu-id="3ab70-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3ab70-120">Type</span></span> | <span data-ttu-id="3ab70-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3ab70-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="3ab70-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ab70-122">Authorization</span></span> | <span data-ttu-id="3ab70-123">string</span><span class="sxs-lookup"><span data-stu-id="3ab70-123">string</span></span> | <span data-ttu-id="3ab70-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ab70-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ab70-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ab70-126">Request body</span></span>

<span data-ttu-id="3ab70-127">В тексте запроса добавьте представление объекта [HistoryItem](../resources/projectrome-historyitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ab70-127">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3ab70-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ab70-128">Response</span></span>

<span data-ttu-id="3ab70-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, если был создан `200 OK` historyItem, или если historyItem был заменен.</span><span class="sxs-lookup"><span data-stu-id="3ab70-129">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="3ab70-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3ab70-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3ab70-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ab70-131">Request</span></span>

<span data-ttu-id="3ab70-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ab70-132">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="3ab70-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ab70-133">Response</span></span>

<span data-ttu-id="3ab70-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ab70-134">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.historyItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
