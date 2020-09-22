---
title: Получение Едукатионалактивити
description: Получение свойств и связей объекта Едукатионалактивити.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ad25a59dd3d8dc58a6eaa6c8b74952e238894f9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007927"
---
# <a name="get-educationalactivity"></a><span data-ttu-id="70824-103">Получение Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="70824-103">Get educationalActivity</span></span>

<span data-ttu-id="70824-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70824-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70824-105">Получение свойств и связей объекта [едукатионалактивити](../resources/educationalactivity.md) из профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="70824-105">Retrieve the properties and relationships of an [educationalActivity](../resources/educationalactivity.md) object from a users profile.</span></span>

## <a name="permissions"></a><span data-ttu-id="70824-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70824-106">Permissions</span></span>

<span data-ttu-id="70824-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70824-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70824-109">Permission type</span></span>                        | <span data-ttu-id="70824-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70824-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="70824-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70824-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="70824-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="70824-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="70824-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70824-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70824-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="70824-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="70824-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="70824-115">Application</span></span>                            | <span data-ttu-id="70824-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="70824-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="70824-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70824-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/educationalActivities/{id}
GET /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70824-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70824-118">Optional query parameters</span></span>

<span data-ttu-id="70824-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="70824-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="70824-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="70824-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="70824-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="70824-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70824-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70824-122">Request headers</span></span>

|<span data-ttu-id="70824-123">Имя</span><span class="sxs-lookup"><span data-stu-id="70824-123">Name</span></span>            |<span data-ttu-id="70824-124">Описание</span><span class="sxs-lookup"><span data-stu-id="70824-124">Description</span></span>                  |
|:---------------|:----------------------------|
|<span data-ttu-id="70824-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70824-125">Authorization</span></span>   |<span data-ttu-id="70824-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70824-p103">Bearer {token}. Required.</span></span>    |

## <a name="request-body"></a><span data-ttu-id="70824-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70824-128">Request body</span></span>

<span data-ttu-id="70824-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70824-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70824-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="70824-130">Response</span></span>

<span data-ttu-id="70824-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [едукатионалактивити](../resources/educationalactivity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70824-131">If successful, this method returns a `200 OK` response code and the requested [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70824-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="70824-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70824-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="70824-133">Request</span></span>

<span data-ttu-id="70824-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70824-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70824-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="70824-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationalactivity"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```
# <a name="c"></a>[<span data-ttu-id="70824-136">C#</span><span class="sxs-lookup"><span data-stu-id="70824-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70824-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70824-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70824-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70824-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="70824-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="70824-139">Response</span></span>

<span data-ttu-id="70824-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70824-140">The following is an example of the response.</span></span>

> <span data-ttu-id="70824-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70824-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "description": null,
    "displayName": "Colorado State University",
    "location": {
      "type": "business",
      "postOfficeBox": null,
      "street": "12000 E Prospect Rd",
      "city": "Fort Collins",
      "state": "Colorado",
      "countryOrRegion": "USA",
      "postalCode": "80525"
    },
    "webUrl": "https://www.colostate.edu"
  },
  "program": {
    "abbreviation": "MBA",
    "activities": null,
    "awards": null,
    "description": "Master of Business Administration with a major in Entreprenuership and Finance.",
    "displayName": "Master of Business Administration",
    "fieldsOfStudy": null,
    "grade": "3.9",
    "notes": null,
    "webUrl": "https://biz.colostate.edu"
  },
  "startMonthYear": "Date"
}
```


