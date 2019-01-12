---
title: Создать или заменить historyItem
description: Создание новой или заменить существующий элемент журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 21c4420ff64d105a5512df1f9a57a5e8309413f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913004"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="4def7-103">Создать или заменить historyItem</span><span class="sxs-lookup"><span data-stu-id="4def7-103">Create or replace a historyItem</span></span>

<span data-ttu-id="4def7-104">Создание новой или заменить существующий элемент журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="4def7-104">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="4def7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4def7-105">Permissions</span></span>

<span data-ttu-id="4def7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4def7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4def7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4def7-108">Permission type</span></span>      | <span data-ttu-id="4def7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4def7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4def7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4def7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4def7-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4def7-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4def7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4def7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4def7-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4def7-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4def7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4def7-114">Application</span></span> | <span data-ttu-id="4def7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4def7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4def7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4def7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="4def7-117">Код должен быть идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="4def7-117">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4def7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4def7-118">Request headers</span></span>

|<span data-ttu-id="4def7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4def7-119">Name</span></span> | <span data-ttu-id="4def7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4def7-120">Type</span></span> | <span data-ttu-id="4def7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4def7-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4def7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4def7-122">Authorization</span></span> | <span data-ttu-id="4def7-123">string</span><span class="sxs-lookup"><span data-stu-id="4def7-123">string</span></span> | <span data-ttu-id="4def7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4def7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4def7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4def7-126">Request body</span></span>

<span data-ttu-id="4def7-127">В тексте запроса укажите представление JSON объекта [historyItem](../resources/projectrome-historyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="4def7-127">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4def7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4def7-128">Response</span></span>

<span data-ttu-id="4def7-129">Успешно завершена, этот метод возвращает `201 Created` код ответа, если был создан historyItem или `200 OK` Если historyItem был заменен.</span><span class="sxs-lookup"><span data-stu-id="4def7-129">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="4def7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4def7-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4def7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4def7-131">Request</span></span>

<span data-ttu-id="4def7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4def7-132">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="4def7-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4def7-133">Response</span></span>

<span data-ttu-id="4def7-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4def7-134">Here is an example of the response.</span></span>

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
