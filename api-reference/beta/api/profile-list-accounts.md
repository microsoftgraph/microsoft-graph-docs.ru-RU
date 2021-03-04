---
title: Учетные записи списка
description: Извлечение списка объектов userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 97d8209e6badb9917768513e1db31d7ccaa2d30a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441096"
---
# <a name="list-accounts"></a><span data-ttu-id="42694-103">Учетные записи списка</span><span class="sxs-lookup"><span data-stu-id="42694-103">List accounts</span></span>

<span data-ttu-id="42694-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42694-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42694-105">Извлекает свойства, связанные с учетной записью пользователя из [профиля.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="42694-105">Retrieves properties related to the user's accounts from the [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="42694-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42694-106">Permissions</span></span>

<span data-ttu-id="42694-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42694-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42694-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42694-109">Permission type</span></span>                        | <span data-ttu-id="42694-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42694-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="42694-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42694-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42694-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42694-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="42694-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42694-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42694-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42694-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="42694-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="42694-115">Application</span></span>                            | <span data-ttu-id="42694-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42694-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="42694-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42694-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account
GET /users/{id | userPrincipalName}/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42694-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42694-118">Optional query parameters</span></span>

<span data-ttu-id="42694-119">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="42694-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="42694-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="42694-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="42694-121">Имя</span><span class="sxs-lookup"><span data-stu-id="42694-121">Name</span></span>            |<span data-ttu-id="42694-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42694-122">Value</span></span>    |<span data-ttu-id="42694-123">Описание</span><span class="sxs-lookup"><span data-stu-id="42694-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="42694-124">$filter</span><span class="sxs-lookup"><span data-stu-id="42694-124">$filter</span></span>         |<span data-ttu-id="42694-125">string</span><span class="sxs-lookup"><span data-stu-id="42694-125">string</span></span>   |<span data-ttu-id="42694-126">Ограничивает ответ только теми объектами, которые содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="42694-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="42694-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="42694-127">$orderby</span></span>        |<span data-ttu-id="42694-128">строка</span><span class="sxs-lookup"><span data-stu-id="42694-128">string</span></span>   |<span data-ttu-id="42694-129">По умолчанию объекты в ответе сортируют по их созданному значениюDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="42694-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="42694-130">Вы можете изменить порядок ответа с помощью *параметра $orderby.*</span><span class="sxs-lookup"><span data-stu-id="42694-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="42694-131">$select</span><span class="sxs-lookup"><span data-stu-id="42694-131">$select</span></span>         |<span data-ttu-id="42694-132">string</span><span class="sxs-lookup"><span data-stu-id="42694-132">string</span></span>   |<span data-ttu-id="42694-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="42694-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="42694-135">$skip</span><span class="sxs-lookup"><span data-stu-id="42694-135">$skip</span></span>           |<span data-ttu-id="42694-136">int</span><span class="sxs-lookup"><span data-stu-id="42694-136">int</span></span>      |<span data-ttu-id="42694-137">Пропустить первые n результаты, полезные для paging.</span><span class="sxs-lookup"><span data-stu-id="42694-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="42694-138">$top</span><span class="sxs-lookup"><span data-stu-id="42694-138">$top</span></span>            |<span data-ttu-id="42694-139">int</span><span class="sxs-lookup"><span data-stu-id="42694-139">int</span></span>      |<span data-ttu-id="42694-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="42694-140">Number of results to be returned.</span></span>                                                                                                                                           |


## <a name="request-headers"></a><span data-ttu-id="42694-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42694-141">Request headers</span></span>

| <span data-ttu-id="42694-142">Имя</span><span class="sxs-lookup"><span data-stu-id="42694-142">Name</span></span>           |<span data-ttu-id="42694-143">Описание</span><span class="sxs-lookup"><span data-stu-id="42694-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="42694-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42694-144">Authorization</span></span>  | <span data-ttu-id="42694-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42694-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="42694-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="42694-147">Content-Type</span></span>   | <span data-ttu-id="42694-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42694-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42694-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42694-150">Request body</span></span>

<span data-ttu-id="42694-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42694-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42694-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="42694-152">Response</span></span>

<span data-ttu-id="42694-153">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userAccountInformation](../resources/useraccountinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="42694-153">If successful, this method returns a `200 OK` response code and a collection of [userAccountInformation](../resources/useraccountinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42694-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="42694-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42694-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="42694-155">Request</span></span>

<span data-ttu-id="42694-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42694-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="42694-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="42694-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_account"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account
```
# <a name="c"></a>[<span data-ttu-id="42694-158">C#</span><span class="sxs-lookup"><span data-stu-id="42694-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-account-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42694-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42694-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-account-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42694-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42694-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-account-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42694-161">Java</span><span class="sxs-lookup"><span data-stu-id="42694-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-account-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="42694-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="42694-162">Response</span></span>

<span data-ttu-id="42694-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="42694-163">The following is an example of the response.</span></span>

> <span data-ttu-id="42694-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42694-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation",
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
      "ageGroup": "adult",
      "countryCode": "NO",
      "preferredLanguageTag": null,
      "userPrincipalName": "innocenty.popov@adventureworks.com"
    }
  ]
}
```


