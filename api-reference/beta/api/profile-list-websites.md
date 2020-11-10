---
title: Список веб-сайтов
description: Получение списка объектов Персонвебсите.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 735e55d789a8edcab21c4bbe5fbe3c1b7c8f172f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967349"
---
# <a name="list-websites"></a><span data-ttu-id="80451-103">Список веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="80451-103">List websites</span></span>

<span data-ttu-id="80451-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80451-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80451-105">Получение списка объектов [персонвебсите](../resources/personwebsite.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="80451-105">Retrieve a list of [personWebsite](../resources/personwebsite.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80451-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80451-106">Permissions</span></span>

<span data-ttu-id="80451-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80451-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80451-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80451-109">Permission type</span></span>                        | <span data-ttu-id="80451-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80451-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="80451-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80451-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="80451-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="80451-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="80451-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80451-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80451-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="80451-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="80451-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="80451-115">Application</span></span>                            | <span data-ttu-id="80451-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="80451-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="80451-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80451-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/websites
GET /users/{id | userPrincipalName}/profile/websites
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80451-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="80451-118">Optional query parameters</span></span>

<span data-ttu-id="80451-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="80451-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="80451-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="80451-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="80451-121">Имя</span><span class="sxs-lookup"><span data-stu-id="80451-121">Name</span></span>            |<span data-ttu-id="80451-122">Значение</span><span class="sxs-lookup"><span data-stu-id="80451-122">Value</span></span>    |<span data-ttu-id="80451-123">Описание</span><span class="sxs-lookup"><span data-stu-id="80451-123">Description</span></span>                                                                                                                                                                      |
|:---------------|:--------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="80451-124">$filter</span><span class="sxs-lookup"><span data-stu-id="80451-124">$filter</span></span>         |<span data-ttu-id="80451-125">string</span><span class="sxs-lookup"><span data-stu-id="80451-125">string</span></span>   |<span data-ttu-id="80451-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="80451-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                                  |
|<span data-ttu-id="80451-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="80451-127">$orderby</span></span>        |<span data-ttu-id="80451-128">строка</span><span class="sxs-lookup"><span data-stu-id="80451-128">string</span></span>   |<span data-ttu-id="80451-129">По умолчанию объекты в отклике сортируются по значению **createdDateTime** в запросе.</span><span class="sxs-lookup"><span data-stu-id="80451-129">By default, the objects in the response are sorted by their **createdDateTime** value in a query.</span></span> <span data-ttu-id="80451-130">Вы можете изменить порядок ответа с помощью `$orderby` параметра.</span><span class="sxs-lookup"><span data-stu-id="80451-130">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="80451-131">$select</span><span class="sxs-lookup"><span data-stu-id="80451-131">$select</span></span>         |<span data-ttu-id="80451-132">string</span><span class="sxs-lookup"><span data-stu-id="80451-132">string</span></span>   |<span data-ttu-id="80451-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="80451-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                             |
|<span data-ttu-id="80451-135">$skip</span><span class="sxs-lookup"><span data-stu-id="80451-135">$skip</span></span>           |<span data-ttu-id="80451-136">int</span><span class="sxs-lookup"><span data-stu-id="80451-136">int</span></span>      |<span data-ttu-id="80451-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="80451-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                     |
|<span data-ttu-id="80451-138">$top</span><span class="sxs-lookup"><span data-stu-id="80451-138">$top</span></span>            |<span data-ttu-id="80451-139">int</span><span class="sxs-lookup"><span data-stu-id="80451-139">int</span></span>      |<span data-ttu-id="80451-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="80451-140">Number of results to be returned.</span></span>                                                                                                                                                |

## <a name="request-headers"></a><span data-ttu-id="80451-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="80451-141">Request headers</span></span>

| <span data-ttu-id="80451-142">Имя</span><span class="sxs-lookup"><span data-stu-id="80451-142">Name</span></span>           |<span data-ttu-id="80451-143">Описание</span><span class="sxs-lookup"><span data-stu-id="80451-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="80451-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80451-144">Authorization</span></span>  | <span data-ttu-id="80451-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80451-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="80451-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80451-147">Request body</span></span>

<span data-ttu-id="80451-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80451-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80451-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="80451-149">Response</span></span>

<span data-ttu-id="80451-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [персонвебсите](../resources/personwebsite.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80451-150">If successful, this method returns a `200 OK` response code and a collection of [personWebsite](../resources/personwebsite.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80451-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="80451-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80451-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="80451-152">Request</span></span>

<span data-ttu-id="80451-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80451-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80451-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="80451-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_websites"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/websites
```
# <a name="c"></a>[<span data-ttu-id="80451-155">C#</span><span class="sxs-lookup"><span data-stu-id="80451-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-websites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80451-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80451-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-websites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80451-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80451-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-websites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80451-158">Java</span><span class="sxs-lookup"><span data-stu-id="80451-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-websites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80451-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="80451-159">Response</span></span>

<span data-ttu-id="80451-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80451-160">The following is an example of the response.</span></span>

> <span data-ttu-id="80451-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80451-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite",
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
        "football"
      ],
      "description": "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway",
      "displayName": "Lyn Damer",
      "webUrl": "www.lyndamer.no"
    }
  ]
}
```


