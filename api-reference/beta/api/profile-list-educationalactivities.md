---
title: List educationalActivities
description: Извлечение списка объектов educationalActivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ab8a9800bd6c8517fd4d3fc84b1485549c4ed4ba
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037279"
---
# <a name="list-educationalactivities"></a><span data-ttu-id="b0a0a-103">List educationalActivities</span><span class="sxs-lookup"><span data-stu-id="b0a0a-103">List educationalActivities</span></span>

<span data-ttu-id="b0a0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0a0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0a0a-105">Извлечение списка [объектов educationalActivity](../resources/educationalactivity.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0a-105">Retrieve a list of [educationalActivity](../resources/educationalactivity.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0a0a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0a0a-106">Permissions</span></span>

<span data-ttu-id="b0a0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0a0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0a0a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0a0a-109">Permission type</span></span>                        | <span data-ttu-id="b0a0a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0a0a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b0a0a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0a0a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0a0a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a0a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b0a0a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0a0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0a0a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a0a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b0a0a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0a0a-115">Application</span></span>                            | <span data-ttu-id="b0a0a-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a0a-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b0a0a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0a0a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/educationalActivities
GET /users/{id | userPrincipalName}/profile/educationalActivities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0a0a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0a0a-118">Optional query parameters</span></span>

<span data-ttu-id="b0a0a-119">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="b0a0a-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b0a0a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="b0a0a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b0a0a-121">Name</span></span>            |<span data-ttu-id="b0a0a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b0a0a-122">Value</span></span>    |<span data-ttu-id="b0a0a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b0a0a-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b0a0a-124">$filter</span><span class="sxs-lookup"><span data-stu-id="b0a0a-124">$filter</span></span>         |<span data-ttu-id="b0a0a-125">string</span><span class="sxs-lookup"><span data-stu-id="b0a0a-125">string</span></span>   |<span data-ttu-id="b0a0a-126">Ограничивает ответ только теми объектами, которые содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="b0a0a-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="b0a0a-127">$orderby</span></span>        |<span data-ttu-id="b0a0a-128">строка</span><span class="sxs-lookup"><span data-stu-id="b0a0a-128">string</span></span>   |<span data-ttu-id="b0a0a-129">По умолчанию объекты в ответе сортируют по их созданному значениюDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="b0a0a-130">Вы можете изменить порядок ответа с помощью *параметра $orderby.*</span><span class="sxs-lookup"><span data-stu-id="b0a0a-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="b0a0a-131">$select</span><span class="sxs-lookup"><span data-stu-id="b0a0a-131">$select</span></span>         |<span data-ttu-id="b0a0a-132">string</span><span class="sxs-lookup"><span data-stu-id="b0a0a-132">string</span></span>   |<span data-ttu-id="b0a0a-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="b0a0a-135">$skip</span><span class="sxs-lookup"><span data-stu-id="b0a0a-135">$skip</span></span>           |<span data-ttu-id="b0a0a-136">int</span><span class="sxs-lookup"><span data-stu-id="b0a0a-136">int</span></span>      |<span data-ttu-id="b0a0a-137">Пропустить первые n результаты, полезные для paging.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="b0a0a-138">$top</span><span class="sxs-lookup"><span data-stu-id="b0a0a-138">$top</span></span>            |<span data-ttu-id="b0a0a-139">int</span><span class="sxs-lookup"><span data-stu-id="b0a0a-139">int</span></span>      |<span data-ttu-id="b0a0a-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="b0a0a-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b0a0a-141">Request headers</span></span>

| <span data-ttu-id="b0a0a-142">Имя</span><span class="sxs-lookup"><span data-stu-id="b0a0a-142">Name</span></span>           |<span data-ttu-id="b0a0a-143">Описание</span><span class="sxs-lookup"><span data-stu-id="b0a0a-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b0a0a-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0a0a-144">Authorization</span></span>  | <span data-ttu-id="b0a0a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="b0a0a-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0a0a-147">Request body</span></span>

<span data-ttu-id="b0a0a-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0a0a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0a0a-149">Response</span></span>

<span data-ttu-id="b0a0a-150">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` объектов [educationalActivity](../resources/educationalactivity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-150">If successful, this method returns a `200 OK` response code and a collection of [educationalActivity](../resources/educationalactivity.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0a0a-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="b0a0a-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0a0a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0a0a-152">Request</span></span>

<span data-ttu-id="b0a0a-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0a0a-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0a0a-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationalactivities"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/educationalActivities
```
# <a name="c"></a>[<span data-ttu-id="b0a0a-155">C#</span><span class="sxs-lookup"><span data-stu-id="b0a0a-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0a0a-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0a0a-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0a0a-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0a0a-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0a0a-158">Java</span><span class="sxs-lookup"><span data-stu-id="b0a0a-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationalactivities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0a0a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0a0a-159">Response</span></span>

<span data-ttu-id="b0a0a-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-160">The following is an example of the response.</span></span>

> <span data-ttu-id="b0a0a-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b0a0a-161">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity",
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
  ]
}
```


