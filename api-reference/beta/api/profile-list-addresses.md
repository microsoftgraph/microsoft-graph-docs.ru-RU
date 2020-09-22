---
title: Список адресов
description: Получение Итемаддрессес из свойства навигации Addresses.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 12ae7539b720a5543e37d12c5f592149e7392dd9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034814"
---
# <a name="list-addresses"></a><span data-ttu-id="4e0a9-103">Список адресов</span><span class="sxs-lookup"><span data-stu-id="4e0a9-103">List addresses</span></span>
<span data-ttu-id="4e0a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e0a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e0a9-105">Получение ресурсов [итемаддресс](../resources/itemaddress.md) из свойства навигации **addresses** .</span><span class="sxs-lookup"><span data-stu-id="4e0a9-105">Get the [itemAddress](../resources/itemaddress.md) resources from the **addresses** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e0a9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e0a9-106">Permissions</span></span>

<span data-ttu-id="4e0a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e0a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e0a9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e0a9-109">Permission type</span></span>                        | <span data-ttu-id="4e0a9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e0a9-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="4e0a9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e0a9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e0a9-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4e0a9-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4e0a9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e0a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e0a9-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4e0a9-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4e0a9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e0a9-115">Application</span></span>                            | <span data-ttu-id="4e0a9-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4e0a9-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="4e0a9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e0a9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/addresses
GET /users/{id | userPrincipalName}/profile/addresses
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e0a9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e0a9-118">Optional query parameters</span></span>

<span data-ttu-id="4e0a9-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="4e0a9-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4e0a9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="4e0a9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4e0a9-121">Name</span></span>            |<span data-ttu-id="4e0a9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e0a9-122">Value</span></span>    |<span data-ttu-id="4e0a9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4e0a9-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4e0a9-124">$filter</span><span class="sxs-lookup"><span data-stu-id="4e0a9-124">$filter</span></span>         |<span data-ttu-id="4e0a9-125">string</span><span class="sxs-lookup"><span data-stu-id="4e0a9-125">string</span></span>   |<span data-ttu-id="4e0a9-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="4e0a9-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="4e0a9-127">$orderby</span></span>        |<span data-ttu-id="4e0a9-128">строка</span><span class="sxs-lookup"><span data-stu-id="4e0a9-128">string</span></span>   |<span data-ttu-id="4e0a9-129">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="4e0a9-130">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="4e0a9-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="4e0a9-131">$select</span><span class="sxs-lookup"><span data-stu-id="4e0a9-131">$select</span></span>         |<span data-ttu-id="4e0a9-132">string</span><span class="sxs-lookup"><span data-stu-id="4e0a9-132">string</span></span>   |<span data-ttu-id="4e0a9-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="4e0a9-135">$skip</span><span class="sxs-lookup"><span data-stu-id="4e0a9-135">$skip</span></span>           |<span data-ttu-id="4e0a9-136">int</span><span class="sxs-lookup"><span data-stu-id="4e0a9-136">int</span></span>      |<span data-ttu-id="4e0a9-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="4e0a9-138">$top</span><span class="sxs-lookup"><span data-stu-id="4e0a9-138">$top</span></span>            |<span data-ttu-id="4e0a9-139">int</span><span class="sxs-lookup"><span data-stu-id="4e0a9-139">int</span></span>      |<span data-ttu-id="4e0a9-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="4e0a9-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e0a9-141">Request headers</span></span>
|<span data-ttu-id="4e0a9-142">Имя</span><span class="sxs-lookup"><span data-stu-id="4e0a9-142">Name</span></span>|<span data-ttu-id="4e0a9-143">Описание</span><span class="sxs-lookup"><span data-stu-id="4e0a9-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4e0a9-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e0a9-144">Authorization</span></span>|<span data-ttu-id="4e0a9-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e0a9-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e0a9-147">Request body</span></span>
<span data-ttu-id="4e0a9-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e0a9-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e0a9-149">Response</span></span>

<span data-ttu-id="4e0a9-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [итемаддресс](../resources/itemaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-150">If successful, this method returns a `200 OK` response code and a collection of [itemAddress](../resources/itemaddress.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e0a9-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="4e0a9-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="4e0a9-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e0a9-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemaddresses_from_profile"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/addresses
```
# <a name="c"></a>[<span data-ttu-id="4e0a9-153">C#</span><span class="sxs-lookup"><span data-stu-id="4e0a9-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemaddresses-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e0a9-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e0a9-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemaddresses-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e0a9-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e0a9-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemaddresses-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4e0a9-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e0a9-156">Response</span></span>
<span data-ttu-id="4e0a9-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4e0a9-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemAddress)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
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
      "displayName": "Home",
      "detail": {
        "type": "home",
        "postOfficeBox": null,
        "street": "221B Baker Street",
        "city": "London",
        "state": null,
        "countryOrRegion": "United Kingdom",
        "postalCode": "E14 3TD"
      },
      "geoCoordinates": null
    }
  ]
}
```


