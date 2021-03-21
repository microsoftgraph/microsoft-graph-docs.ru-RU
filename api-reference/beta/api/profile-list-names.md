---
title: Перечисление имен
description: Извлечение списка объектов personName из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a6d3dadfb3b8565519adf7fc1c95ee593bb57d83
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957209"
---
# <a name="list-names"></a><span data-ttu-id="87d7b-103">Перечисление имен</span><span class="sxs-lookup"><span data-stu-id="87d7b-103">List names</span></span>

<span data-ttu-id="87d7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87d7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87d7b-105">Извлечение списка [объектов personName](../resources/personname.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="87d7b-105">Retrieve a list of [personName](../resources/personname.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87d7b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87d7b-106">Permissions</span></span>

<span data-ttu-id="87d7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87d7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87d7b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87d7b-109">Permission type</span></span>                        | <span data-ttu-id="87d7b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87d7b-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="87d7b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87d7b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87d7b-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87d7b-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="87d7b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87d7b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87d7b-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87d7b-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="87d7b-115">Application</span><span class="sxs-lookup"><span data-stu-id="87d7b-115">Application</span></span>                            | <span data-ttu-id="87d7b-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87d7b-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="87d7b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87d7b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names
GET /users/{id | userPrincipalName}/profile/names
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87d7b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="87d7b-118">Optional query parameters</span></span>

<span data-ttu-id="87d7b-119">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="87d7b-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="87d7b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="87d7b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="87d7b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="87d7b-121">Name</span></span>            |<span data-ttu-id="87d7b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87d7b-122">Value</span></span>    |<span data-ttu-id="87d7b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="87d7b-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="87d7b-124">$filter</span><span class="sxs-lookup"><span data-stu-id="87d7b-124">$filter</span></span>         |<span data-ttu-id="87d7b-125">string</span><span class="sxs-lookup"><span data-stu-id="87d7b-125">string</span></span>   |<span data-ttu-id="87d7b-126">Ограничивает ответ только теми объектами, которые содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="87d7b-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="87d7b-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="87d7b-127">$orderby</span></span>        |<span data-ttu-id="87d7b-128">строка</span><span class="sxs-lookup"><span data-stu-id="87d7b-128">string</span></span>   |<span data-ttu-id="87d7b-129">По умолчанию объекты в ответе сортируют по их созданному значениюDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="87d7b-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="87d7b-130">Вы можете изменить порядок ответа с помощью *параметра $orderby.*</span><span class="sxs-lookup"><span data-stu-id="87d7b-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="87d7b-131">$select</span><span class="sxs-lookup"><span data-stu-id="87d7b-131">$select</span></span>         |<span data-ttu-id="87d7b-132">string</span><span class="sxs-lookup"><span data-stu-id="87d7b-132">string</span></span>   |<span data-ttu-id="87d7b-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="87d7b-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="87d7b-135">$skip</span><span class="sxs-lookup"><span data-stu-id="87d7b-135">$skip</span></span>           |<span data-ttu-id="87d7b-136">int</span><span class="sxs-lookup"><span data-stu-id="87d7b-136">int</span></span>      |<span data-ttu-id="87d7b-137">Пропустить первые n результаты, полезные для paging.</span><span class="sxs-lookup"><span data-stu-id="87d7b-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="87d7b-138">$top</span><span class="sxs-lookup"><span data-stu-id="87d7b-138">$top</span></span>            |<span data-ttu-id="87d7b-139">int</span><span class="sxs-lookup"><span data-stu-id="87d7b-139">int</span></span>      |<span data-ttu-id="87d7b-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="87d7b-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="87d7b-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87d7b-141">Request headers</span></span>

| <span data-ttu-id="87d7b-142">Имя</span><span class="sxs-lookup"><span data-stu-id="87d7b-142">Name</span></span>           |<span data-ttu-id="87d7b-143">Описание</span><span class="sxs-lookup"><span data-stu-id="87d7b-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="87d7b-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87d7b-144">Authorization</span></span>  | <span data-ttu-id="87d7b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87d7b-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="87d7b-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87d7b-147">Content-Type</span></span>   | <span data-ttu-id="87d7b-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87d7b-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87d7b-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87d7b-150">Request body</span></span>

<span data-ttu-id="87d7b-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87d7b-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87d7b-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="87d7b-152">Response</span></span>

<span data-ttu-id="87d7b-153">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [personName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87d7b-153">If successful, this method returns a `200 OK` response code and a collection of [personName](../resources/personname.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87d7b-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="87d7b-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="87d7b-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="87d7b-155">Request</span></span>

<span data-ttu-id="87d7b-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87d7b-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87d7b-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="87d7b-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_names_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names
```
# <a name="c"></a>[<span data-ttu-id="87d7b-158">C#</span><span class="sxs-lookup"><span data-stu-id="87d7b-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-names-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87d7b-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87d7b-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-names-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87d7b-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87d7b-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-names-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87d7b-161">Java</span><span class="sxs-lookup"><span data-stu-id="87d7b-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-names-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="87d7b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="87d7b-162">Response</span></span>

<span data-ttu-id="87d7b-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="87d7b-163">The following is an example of the response.</span></span>

> <span data-ttu-id="87d7b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87d7b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName",
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
      "displayName": "Innocenty Popov",
      "first": "Innocenty",
      "initials": "IP",
      "last": "Popov",
      "languageTag": "en-US",
      "maiden": null,
      "middle": null,
      "nickname": "Kesha",
      "suffix": null,
      "title": null,
      "pronunciation": {
        "displayName": "In-no ken-te ",
        "first": "In-no ken-te Pop-ov",
        "maiden": null,
        "middle": null,
        "last": "Pop-ov"
      }
    }
  ]
}
```


