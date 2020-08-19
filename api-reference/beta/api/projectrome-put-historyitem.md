---
title: Создание или замена объекта historyItem
description: Создание нового или замена существующего элемента журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: c1ba6a574f106fd095da4c16ecc5a9826a1ec90d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809931"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="c7d1d-103">Создание или замена объекта historyItem</span><span class="sxs-lookup"><span data-stu-id="c7d1d-103">Create or replace a historyItem</span></span>

<span data-ttu-id="c7d1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7d1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7d1d-105">Создание нового или замена существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7d1d-105">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7d1d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7d1d-106">Permissions</span></span>

<span data-ttu-id="c7d1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7d1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c7d1d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7d1d-109">Permission type</span></span>      | <span data-ttu-id="c7d1d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7d1d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7d1d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7d1d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7d1d-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c7d1d-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c7d1d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7d1d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7d1d-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c7d1d-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c7d1d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7d1d-115">Application</span></span> | <span data-ttu-id="c7d1d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7d1d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7d1d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7d1d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="c7d1d-118">Идентификатор должен быть идентификатором GUID.</span><span class="sxs-lookup"><span data-stu-id="c7d1d-118">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7d1d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7d1d-119">Request headers</span></span>

|<span data-ttu-id="c7d1d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c7d1d-120">Name</span></span> | <span data-ttu-id="c7d1d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c7d1d-121">Type</span></span> | <span data-ttu-id="c7d1d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c7d1d-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="c7d1d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7d1d-123">Authorization</span></span> | <span data-ttu-id="c7d1d-124">string</span><span class="sxs-lookup"><span data-stu-id="c7d1d-124">string</span></span> | <span data-ttu-id="c7d1d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7d1d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7d1d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7d1d-127">Request body</span></span>

<span data-ttu-id="c7d1d-128">В тексте запроса добавьте представление объекта [historyItem](../resources/projectrome-historyitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7d1d-128">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c7d1d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7d1d-129">Response</span></span>

<span data-ttu-id="c7d1d-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, если был создан historyItem, или `200 OK` Если historyItem был заменен.</span><span class="sxs-lookup"><span data-stu-id="c7d1d-130">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="c7d1d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c7d1d-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c7d1d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7d1d-132">Request</span></span>

<span data-ttu-id="c7d1d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7d1d-133">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c7d1d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7d1d-134">Response</span></span>

<span data-ttu-id="c7d1d-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7d1d-135">Here is an example of the response.</span></span>

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
