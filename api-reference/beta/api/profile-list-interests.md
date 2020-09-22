---
title: Список интересов
description: Получение списка объектов Персонинтерест.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fbaeb9b1b3aadda736d3685753cac295667b8fcf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034773"
---
# <a name="list-interests"></a><span data-ttu-id="e8395-103">Список интересов</span><span class="sxs-lookup"><span data-stu-id="e8395-103">List interests</span></span>

<span data-ttu-id="e8395-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8395-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8395-105">Получение списка объектов [персонинтерест](../resources/personinterest.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8395-105">Retrieve a list of [personInterest](../resources/personinterest.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8395-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8395-106">Permissions</span></span>

<span data-ttu-id="e8395-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8395-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8395-109">Permission type</span></span>                        | <span data-ttu-id="e8395-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8395-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e8395-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8395-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8395-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e8395-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e8395-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8395-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8395-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e8395-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e8395-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8395-115">Application</span></span>                            | <span data-ttu-id="e8395-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e8395-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="e8395-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8395-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/interests
GET /users/{id | userPrincipalName}/profile/interests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8395-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e8395-118">Optional query parameters</span></span>

<span data-ttu-id="e8395-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e8395-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8395-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8395-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="e8395-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e8395-121">Name</span></span>            |<span data-ttu-id="e8395-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8395-122">Value</span></span>    |<span data-ttu-id="e8395-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e8395-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e8395-124">$filter</span><span class="sxs-lookup"><span data-stu-id="e8395-124">$filter</span></span>         |<span data-ttu-id="e8395-125">string</span><span class="sxs-lookup"><span data-stu-id="e8395-125">string</span></span>   |<span data-ttu-id="e8395-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="e8395-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="e8395-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="e8395-127">$orderby</span></span>        |<span data-ttu-id="e8395-128">строка</span><span class="sxs-lookup"><span data-stu-id="e8395-128">string</span></span>   |<span data-ttu-id="e8395-129">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="e8395-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="e8395-130">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="e8395-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="e8395-131">$select</span><span class="sxs-lookup"><span data-stu-id="e8395-131">$select</span></span>         |<span data-ttu-id="e8395-132">string</span><span class="sxs-lookup"><span data-stu-id="e8395-132">string</span></span>   |<span data-ttu-id="e8395-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="e8395-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="e8395-135">$skip</span><span class="sxs-lookup"><span data-stu-id="e8395-135">$skip</span></span>           |<span data-ttu-id="e8395-136">int</span><span class="sxs-lookup"><span data-stu-id="e8395-136">int</span></span>      |<span data-ttu-id="e8395-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="e8395-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="e8395-138">$top</span><span class="sxs-lookup"><span data-stu-id="e8395-138">$top</span></span>            |<span data-ttu-id="e8395-139">int</span><span class="sxs-lookup"><span data-stu-id="e8395-139">int</span></span>      |<span data-ttu-id="e8395-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="e8395-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="e8395-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e8395-141">Request headers</span></span>

| <span data-ttu-id="e8395-142">Имя</span><span class="sxs-lookup"><span data-stu-id="e8395-142">Name</span></span>           |<span data-ttu-id="e8395-143">Описание</span><span class="sxs-lookup"><span data-stu-id="e8395-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e8395-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8395-144">Authorization</span></span>  | <span data-ttu-id="e8395-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8395-p105">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="e8395-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8395-147">Request body</span></span>

<span data-ttu-id="e8395-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8395-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8395-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8395-149">Response</span></span>

<span data-ttu-id="e8395-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [персонинтерест](../resources/personinterest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8395-150">If successful, this method returns a `200 OK` response code and a collection of [personInterest](../resources/personinterest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8395-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8395-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8395-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8395-152">Request</span></span>

<span data-ttu-id="e8395-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8395-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8395-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8395-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_interests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/interests
```
# <a name="c"></a>[<span data-ttu-id="e8395-155">C#</span><span class="sxs-lookup"><span data-stu-id="e8395-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8395-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8395-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8395-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8395-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8395-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8395-158">Response</span></span>

<span data-ttu-id="e8395-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8395-159">The following is an example of the response.</span></span>

> <span data-ttu-id="e8395-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8395-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest",
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
      "categories": [
        "Sports"
      ],
      "description": "World's greatest football club",
      "displayName": "Chelsea FC",
      "webUrl": "https://www.chelseafc.com",
      "collaborationTags": null
    }
  ]
}
```


