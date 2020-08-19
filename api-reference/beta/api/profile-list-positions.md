---
title: Позиции списка
description: Получение списка объектов Воркпоситион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 60770c962298a764b686c6fa7c578c69e95dc0ec
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810687"
---
# <a name="list-positions"></a><span data-ttu-id="b1aad-103">Позиции списка</span><span class="sxs-lookup"><span data-stu-id="b1aad-103">List positions</span></span>

<span data-ttu-id="b1aad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1aad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1aad-105">Получение списка объектов [воркпоситион](../resources/workposition.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1aad-105">Retrieve a list of [workPosition](../resources/workposition.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b1aad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1aad-106">Permissions</span></span>

<span data-ttu-id="b1aad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1aad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1aad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1aad-109">Permission type</span></span>                        | <span data-ttu-id="b1aad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1aad-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b1aad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1aad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1aad-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b1aad-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b1aad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1aad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1aad-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b1aad-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b1aad-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b1aad-115">Application</span></span>                            | <span data-ttu-id="b1aad-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b1aad-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b1aad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1aad-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/positions
GET /users/{id | userPrincipalName}/profile/positions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1aad-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1aad-118">Optional query parameters</span></span>

<span data-ttu-id="b1aad-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b1aad-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="b1aad-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b1aad-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="b1aad-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b1aad-121">Name</span></span>            |<span data-ttu-id="b1aad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b1aad-122">Value</span></span>    |<span data-ttu-id="b1aad-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b1aad-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b1aad-124">$filter</span><span class="sxs-lookup"><span data-stu-id="b1aad-124">$filter</span></span>         |<span data-ttu-id="b1aad-125">string</span><span class="sxs-lookup"><span data-stu-id="b1aad-125">string</span></span>   |<span data-ttu-id="b1aad-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="b1aad-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="b1aad-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="b1aad-127">$orderby</span></span>        |<span data-ttu-id="b1aad-128">строка</span><span class="sxs-lookup"><span data-stu-id="b1aad-128">string</span></span>   |<span data-ttu-id="b1aad-129">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="b1aad-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="b1aad-130">Вы можете изменить порядок ответа с помощью `$orderby` параметра.</span><span class="sxs-lookup"><span data-stu-id="b1aad-130">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="b1aad-131">$select</span><span class="sxs-lookup"><span data-stu-id="b1aad-131">$select</span></span>         |<span data-ttu-id="b1aad-132">string</span><span class="sxs-lookup"><span data-stu-id="b1aad-132">string</span></span>   |<span data-ttu-id="b1aad-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="b1aad-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="b1aad-135">$skip</span><span class="sxs-lookup"><span data-stu-id="b1aad-135">$skip</span></span>           |<span data-ttu-id="b1aad-136">int</span><span class="sxs-lookup"><span data-stu-id="b1aad-136">int</span></span>      |<span data-ttu-id="b1aad-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="b1aad-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="b1aad-138">$top</span><span class="sxs-lookup"><span data-stu-id="b1aad-138">$top</span></span>            |<span data-ttu-id="b1aad-139">int</span><span class="sxs-lookup"><span data-stu-id="b1aad-139">int</span></span>      |<span data-ttu-id="b1aad-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="b1aad-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="b1aad-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1aad-141">Request headers</span></span>

| <span data-ttu-id="b1aad-142">Имя</span><span class="sxs-lookup"><span data-stu-id="b1aad-142">Name</span></span>           |<span data-ttu-id="b1aad-143">Описание</span><span class="sxs-lookup"><span data-stu-id="b1aad-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b1aad-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1aad-144">Authorization</span></span>  | <span data-ttu-id="b1aad-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1aad-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="b1aad-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1aad-147">Request body</span></span>

<span data-ttu-id="b1aad-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1aad-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1aad-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1aad-149">Response</span></span>

<span data-ttu-id="b1aad-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркпоситион](../resources/workposition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1aad-150">If successful, this method returns a `200 OK` response code and a collection of [workPosition](../resources/workposition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1aad-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="b1aad-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1aad-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1aad-152">Request</span></span>

<span data-ttu-id="b1aad-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1aad-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1aad-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1aad-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_positions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/positions
```
# <a name="c"></a>[<span data-ttu-id="b1aad-155">C#</span><span class="sxs-lookup"><span data-stu-id="b1aad-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-positions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1aad-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1aad-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-positions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1aad-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1aad-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-positions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b1aad-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1aad-158">Response</span></span>

<span data-ttu-id="b1aad-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1aad-159">The following is an example of the response.</span></span>

> <span data-ttu-id="b1aad-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1aad-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List positions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
