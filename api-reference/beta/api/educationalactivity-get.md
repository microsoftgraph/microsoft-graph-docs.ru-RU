---
title: Получение Едукатионалактивити
description: Получение свойств и связей объекта едукатионалактивити.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 980f7f246ec40a8822502c3c22497ee408f2fe8c
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994795"
---
# <a name="get-educationalactivity"></a><span data-ttu-id="0945b-103">Получение Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="0945b-103">Get educationalActivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0945b-104">Получение свойств и связей объекта [едукатионалактивити](../resources/educationalactivity.md) из профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="0945b-104">Retrieve the properties and relationships of an [educationalActivity](../resources/educationalactivity.md) object from a users profile.</span></span>

## <a name="permissions"></a><span data-ttu-id="0945b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0945b-105">Permissions</span></span>

<span data-ttu-id="0945b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0945b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0945b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0945b-108">Permission type</span></span>                        | <span data-ttu-id="0945b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0945b-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="0945b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0945b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0945b-111">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0945b-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0945b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0945b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0945b-113">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0945b-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0945b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0945b-114">Application</span></span>                            | <span data-ttu-id="0945b-115">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0945b-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="0945b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0945b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/educationalActivities/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0945b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0945b-117">Optional query parameters</span></span>

<span data-ttu-id="0945b-118">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0945b-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="0945b-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0945b-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="0945b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0945b-120">Name</span></span>            |<span data-ttu-id="0945b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0945b-121">Value</span></span>    |<span data-ttu-id="0945b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0945b-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="0945b-123">$filter</span><span class="sxs-lookup"><span data-stu-id="0945b-123">$filter</span></span>         |<span data-ttu-id="0945b-124">string</span><span class="sxs-lookup"><span data-stu-id="0945b-124">string</span></span>   |<span data-ttu-id="0945b-125">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="0945b-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="0945b-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="0945b-126">$orderby</span></span>        |<span data-ttu-id="0945b-127">строка</span><span class="sxs-lookup"><span data-stu-id="0945b-127">string</span></span>   |<span data-ttu-id="0945b-128">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="0945b-128">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="0945b-129">Вы можете изменить порядок ответа с помощью `$orderby` параметра.</span><span class="sxs-lookup"><span data-stu-id="0945b-129">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="0945b-130">$select</span><span class="sxs-lookup"><span data-stu-id="0945b-130">$select</span></span>         |<span data-ttu-id="0945b-131">string</span><span class="sxs-lookup"><span data-stu-id="0945b-131">string</span></span>   |<span data-ttu-id="0945b-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="0945b-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="0945b-134">$skip</span><span class="sxs-lookup"><span data-stu-id="0945b-134">$skip</span></span>           |<span data-ttu-id="0945b-135">int</span><span class="sxs-lookup"><span data-stu-id="0945b-135">int</span></span>      |<span data-ttu-id="0945b-136">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="0945b-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="0945b-137">$top</span><span class="sxs-lookup"><span data-stu-id="0945b-137">$top</span></span>            |<span data-ttu-id="0945b-138">int</span><span class="sxs-lookup"><span data-stu-id="0945b-138">int</span></span>      |<span data-ttu-id="0945b-139">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="0945b-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="0945b-140">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0945b-140">Request headers</span></span>

| <span data-ttu-id="0945b-141">Имя</span><span class="sxs-lookup"><span data-stu-id="0945b-141">Name</span></span>           |<span data-ttu-id="0945b-142">Описание</span><span class="sxs-lookup"><span data-stu-id="0945b-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0945b-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0945b-143">Authorization</span></span>  | <span data-ttu-id="0945b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0945b-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="0945b-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0945b-146">Request body</span></span>

<span data-ttu-id="0945b-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0945b-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0945b-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="0945b-148">Response</span></span>

<span data-ttu-id="0945b-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [едукатионалактивити](../resources/educationalactivity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0945b-149">If successful, this method returns a `200 OK` response code and the requested [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0945b-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="0945b-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0945b-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0945b-151">Request</span></span>

<span data-ttu-id="0945b-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0945b-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0945b-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="0945b-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationalactivity"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0945b-154">C#</span><span class="sxs-lookup"><span data-stu-id="0945b-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0945b-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0945b-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0945b-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0945b-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0945b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="0945b-157">Response</span></span>

<span data-ttu-id="0945b-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0945b-158">The following is an example of the response.</span></span>

> <span data-ttu-id="0945b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0945b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
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
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
