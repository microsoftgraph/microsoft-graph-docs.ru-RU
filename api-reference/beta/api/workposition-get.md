---
title: Получение Воркпоситион
description: Получение свойств и связей объекта Воркпоситион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9a600be212907e12d03329aa3027c86d41b726ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092960"
---
# <a name="get-workposition"></a><span data-ttu-id="1f963-103">Получение Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="1f963-103">Get workPosition</span></span>

<span data-ttu-id="1f963-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f963-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f963-105">Получение свойств и связей объекта [воркпоситион](../resources/workposition.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f963-105">Retrieve the properties and relationships of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f963-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f963-106">Permissions</span></span>

<span data-ttu-id="1f963-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f963-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f963-109">Permission type</span></span>                        | <span data-ttu-id="1f963-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f963-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="1f963-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f963-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f963-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1f963-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1f963-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f963-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f963-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1f963-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1f963-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f963-115">Application</span></span>                            | <span data-ttu-id="1f963-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1f963-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="1f963-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f963-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/positions/{id}
GET /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f963-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f963-118">Optional query parameters</span></span>

<span data-ttu-id="1f963-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="1f963-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="1f963-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="1f963-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="1f963-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="1f963-121">For optimal performance, only select the subset of properties needed.</span></span>                                                                                                                                         |

## <a name="request-headers"></a><span data-ttu-id="1f963-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f963-122">Request headers</span></span>

| <span data-ttu-id="1f963-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1f963-123">Name</span></span>           |<span data-ttu-id="1f963-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1f963-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="1f963-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f963-125">Authorization</span></span>  | <span data-ttu-id="1f963-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f963-p103">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="1f963-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f963-128">Request body</span></span>

<span data-ttu-id="1f963-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f963-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f963-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f963-130">Response</span></span>

<span data-ttu-id="1f963-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркпоситион](../resources/workposition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f963-131">If successful, this method returns a `200 OK` response code and the requested [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f963-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="1f963-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f963-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f963-133">Request</span></span>

<span data-ttu-id="1f963-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f963-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f963-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f963-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workposition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/positions/{id}
```
# <a name="c"></a>[<span data-ttu-id="1f963-136">C#</span><span class="sxs-lookup"><span data-stu-id="1f963-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f963-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f963-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f963-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f963-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f963-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f963-139">Response</span></span>

<span data-ttu-id="1f963-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f963-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1f963-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f963-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
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
  "categories": null,
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "postOfficeBox": null,
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "state": null,
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "description": null,
    "endMonthYear": null,
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting",
    "startMonthYear": "datetime-value",
    "summary": null
  },
  "manager": null,
  "colleagues": null,
  "isCurrent": true
}
```


