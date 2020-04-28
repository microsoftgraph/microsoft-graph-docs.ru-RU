---
title: Создание или замена объекта historyItem
description: Создание нового или замена существующего элемента журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: 9d7f6d7888ba8a14f16e3756c4c01c3a16c3d73a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454880"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="5637e-103">Создание или замена объекта historyItem</span><span class="sxs-lookup"><span data-stu-id="5637e-103">Create or replace a historyItem</span></span>

<span data-ttu-id="5637e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5637e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5637e-105">Создание нового или замена существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="5637e-105">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="5637e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5637e-106">Permissions</span></span>

<span data-ttu-id="5637e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5637e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5637e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5637e-109">Permission type</span></span>      | <span data-ttu-id="5637e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5637e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5637e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5637e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5637e-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5637e-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5637e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5637e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5637e-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5637e-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5637e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5637e-115">Application</span></span> | <span data-ttu-id="5637e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5637e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5637e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5637e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="5637e-118">Идентификатор должен быть идентификатором GUID.</span><span class="sxs-lookup"><span data-stu-id="5637e-118">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5637e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5637e-119">Request headers</span></span>

|<span data-ttu-id="5637e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5637e-120">Name</span></span> | <span data-ttu-id="5637e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5637e-121">Type</span></span> | <span data-ttu-id="5637e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5637e-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="5637e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5637e-123">Authorization</span></span> | <span data-ttu-id="5637e-124">string</span><span class="sxs-lookup"><span data-stu-id="5637e-124">string</span></span> | <span data-ttu-id="5637e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5637e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5637e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5637e-127">Request body</span></span>

<span data-ttu-id="5637e-128">В тексте запроса добавьте представление объекта [historyItem](../resources/projectrome-historyitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5637e-128">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5637e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5637e-129">Response</span></span>

<span data-ttu-id="5637e-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, если был создан `200 OK` historyItem, или если historyItem был заменен.</span><span class="sxs-lookup"><span data-stu-id="5637e-130">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="5637e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5637e-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5637e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5637e-132">Request</span></span>

<span data-ttu-id="5637e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5637e-133">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="5637e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5637e-134">Response</span></span>

<span data-ttu-id="5637e-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5637e-135">Here is an example of the response.</span></span>

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
