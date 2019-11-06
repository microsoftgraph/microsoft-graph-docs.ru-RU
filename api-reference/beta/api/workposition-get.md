---
title: Получение Воркпоситион
description: Получение свойств и связей объекта Воркпоситион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 12029bd8bb74f98fc52cde7a5337b09fc40053b7
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997425"
---
# <a name="get-workposition"></a><span data-ttu-id="a42c7-103">Получение Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="a42c7-103">Get workPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a42c7-104">Получение свойств и связей объекта [воркпоситион](../resources/workposition.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="a42c7-104">Retrieve the properties and relationships of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a42c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a42c7-105">Permissions</span></span>

<span data-ttu-id="a42c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a42c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a42c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a42c7-108">Permission type</span></span>                        | <span data-ttu-id="a42c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a42c7-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="a42c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a42c7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a42c7-111">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a42c7-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a42c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a42c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a42c7-113">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a42c7-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a42c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a42c7-114">Application</span></span>                            | <span data-ttu-id="a42c7-115">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a42c7-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="a42c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a42c7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/positions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a42c7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a42c7-117">Optional query parameters</span></span>

<span data-ttu-id="a42c7-118">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a42c7-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="a42c7-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a42c7-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="a42c7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a42c7-120">Name</span></span>            |<span data-ttu-id="a42c7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a42c7-121">Value</span></span>    |<span data-ttu-id="a42c7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a42c7-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="a42c7-123">$filter</span><span class="sxs-lookup"><span data-stu-id="a42c7-123">$filter</span></span>         |<span data-ttu-id="a42c7-124">string</span><span class="sxs-lookup"><span data-stu-id="a42c7-124">string</span></span>   |<span data-ttu-id="a42c7-125">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="a42c7-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="a42c7-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="a42c7-126">$orderby</span></span>        |<span data-ttu-id="a42c7-127">строка</span><span class="sxs-lookup"><span data-stu-id="a42c7-127">string</span></span>   |<span data-ttu-id="a42c7-128">По умолчанию объекты в отклике сортируются по значению **createdDateTime** в запросе.</span><span class="sxs-lookup"><span data-stu-id="a42c7-128">By default, the objects in the response are sorted by their **createdDateTime** value in a query.</span></span> <span data-ttu-id="a42c7-129">Вы можете изменить порядок ответа с помощью `$orderby` параметра.</span><span class="sxs-lookup"><span data-stu-id="a42c7-129">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="a42c7-130">$select</span><span class="sxs-lookup"><span data-stu-id="a42c7-130">$select</span></span>         |<span data-ttu-id="a42c7-131">string</span><span class="sxs-lookup"><span data-stu-id="a42c7-131">string</span></span>   |<span data-ttu-id="a42c7-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="a42c7-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="a42c7-134">$skip</span><span class="sxs-lookup"><span data-stu-id="a42c7-134">$skip</span></span>           |<span data-ttu-id="a42c7-135">int</span><span class="sxs-lookup"><span data-stu-id="a42c7-135">int</span></span>      |<span data-ttu-id="a42c7-136">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="a42c7-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="a42c7-137">$top</span><span class="sxs-lookup"><span data-stu-id="a42c7-137">$top</span></span>            |<span data-ttu-id="a42c7-138">int</span><span class="sxs-lookup"><span data-stu-id="a42c7-138">int</span></span>      |<span data-ttu-id="a42c7-139">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="a42c7-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="a42c7-140">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a42c7-140">Request headers</span></span>

| <span data-ttu-id="a42c7-141">Имя</span><span class="sxs-lookup"><span data-stu-id="a42c7-141">Name</span></span>           |<span data-ttu-id="a42c7-142">Описание</span><span class="sxs-lookup"><span data-stu-id="a42c7-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a42c7-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a42c7-143">Authorization</span></span>  | <span data-ttu-id="a42c7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a42c7-p105">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="a42c7-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a42c7-146">Request body</span></span>

<span data-ttu-id="a42c7-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a42c7-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a42c7-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="a42c7-148">Response</span></span>

<span data-ttu-id="a42c7-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркпоситион](../resources/workposition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a42c7-149">If successful, this method returns a `200 OK` response code and the requested [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a42c7-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="a42c7-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a42c7-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="a42c7-151">Request</span></span>

<span data-ttu-id="a42c7-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a42c7-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a42c7-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="a42c7-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workposition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/positions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a42c7-154">C#</span><span class="sxs-lookup"><span data-stu-id="a42c7-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a42c7-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a42c7-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a42c7-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a42c7-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a42c7-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a42c7-157">Response</span></span>

<span data-ttu-id="a42c7-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a42c7-158">The following is an example of the response.</span></span>

> <span data-ttu-id="a42c7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a42c7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
