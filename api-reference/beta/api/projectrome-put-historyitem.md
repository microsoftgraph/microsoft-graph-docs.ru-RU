---
title: Создать или заменить historyItem
description: Создание новой или заменить существующий элемент журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 6ea4a45f2b9d0021bb339e8edadd9006042a9456
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929699"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="15c4e-103">Создать или заменить historyItem</span><span class="sxs-lookup"><span data-stu-id="15c4e-103">Create or replace a historyItem</span></span>

> <span data-ttu-id="15c4e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15c4e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15c4e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c4e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15c4e-106">Создание новой или заменить существующий элемент журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="15c4e-106">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="15c4e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15c4e-107">Permissions</span></span>

<span data-ttu-id="15c4e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15c4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="15c4e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15c4e-110">Permission type</span></span>      | <span data-ttu-id="15c4e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15c4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15c4e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15c4e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15c4e-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="15c4e-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="15c4e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15c4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15c4e-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="15c4e-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="15c4e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15c4e-116">Application</span></span> | <span data-ttu-id="15c4e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c4e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15c4e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15c4e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="15c4e-119">Код должен быть идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="15c4e-119">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15c4e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15c4e-120">Request headers</span></span>

|<span data-ttu-id="15c4e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="15c4e-121">Name</span></span> | <span data-ttu-id="15c4e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="15c4e-122">Type</span></span> | <span data-ttu-id="15c4e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="15c4e-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="15c4e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="15c4e-124">Authorization</span></span> | <span data-ttu-id="15c4e-125">строка</span><span class="sxs-lookup"><span data-stu-id="15c4e-125">string</span></span> | <span data-ttu-id="15c4e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15c4e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15c4e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15c4e-128">Request body</span></span>

<span data-ttu-id="15c4e-129">В тексте запроса укажите представление JSON объекта [historyItem](../resources/projectrome-historyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="15c4e-129">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="15c4e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="15c4e-130">Response</span></span>

<span data-ttu-id="15c4e-131">Успешно завершена, этот метод возвращает `201 Created` код ответа, если был создан historyItem или `200 OK` Если historyItem был заменен.</span><span class="sxs-lookup"><span data-stu-id="15c4e-131">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="15c4e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="15c4e-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="15c4e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="15c4e-133">Request</span></span>

<span data-ttu-id="15c4e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15c4e-134">Here is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="15c4e-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="15c4e-135">Response</span></span>

<span data-ttu-id="15c4e-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15c4e-136">Here is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
