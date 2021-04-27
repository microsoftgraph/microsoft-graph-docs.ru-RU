---
title: Интересы списка
description: Извлечение списка объектов personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fb2d4de0dc98960c3a43d80e65131d7ba926b59a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037251"
---
# <a name="list-interests"></a><span data-ttu-id="adf14-103">Интересы списка</span><span class="sxs-lookup"><span data-stu-id="adf14-103">List interests</span></span>

<span data-ttu-id="adf14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adf14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adf14-105">Извлечение списка [объектов personInterest](../resources/personinterest.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="adf14-105">Retrieve a list of [personInterest](../resources/personinterest.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="adf14-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="adf14-106">Permissions</span></span>

<span data-ttu-id="adf14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adf14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adf14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adf14-109">Permission type</span></span>                        | <span data-ttu-id="adf14-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="adf14-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="adf14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adf14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="adf14-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adf14-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="adf14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adf14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adf14-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adf14-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="adf14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adf14-115">Application</span></span>                            | <span data-ttu-id="adf14-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adf14-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="adf14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adf14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/interests
GET /users/{id | userPrincipalName}/profile/interests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adf14-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="adf14-118">Optional query parameters</span></span>

<span data-ttu-id="adf14-119">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="adf14-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="adf14-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="adf14-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="adf14-121">Имя</span><span class="sxs-lookup"><span data-stu-id="adf14-121">Name</span></span>            |<span data-ttu-id="adf14-122">Значение</span><span class="sxs-lookup"><span data-stu-id="adf14-122">Value</span></span>    |<span data-ttu-id="adf14-123">Описание</span><span class="sxs-lookup"><span data-stu-id="adf14-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="adf14-124">$filter</span><span class="sxs-lookup"><span data-stu-id="adf14-124">$filter</span></span>         |<span data-ttu-id="adf14-125">string</span><span class="sxs-lookup"><span data-stu-id="adf14-125">string</span></span>   |<span data-ttu-id="adf14-126">Ограничивает ответ только теми объектами, которые содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="adf14-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="adf14-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="adf14-127">$orderby</span></span>        |<span data-ttu-id="adf14-128">строка</span><span class="sxs-lookup"><span data-stu-id="adf14-128">string</span></span>   |<span data-ttu-id="adf14-129">По умолчанию объекты в ответе сортируют по их созданному значениюDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="adf14-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="adf14-130">Вы можете изменить порядок ответа с помощью *параметра $orderby.*</span><span class="sxs-lookup"><span data-stu-id="adf14-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="adf14-131">$select</span><span class="sxs-lookup"><span data-stu-id="adf14-131">$select</span></span>         |<span data-ttu-id="adf14-132">string</span><span class="sxs-lookup"><span data-stu-id="adf14-132">string</span></span>   |<span data-ttu-id="adf14-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="adf14-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="adf14-135">$skip</span><span class="sxs-lookup"><span data-stu-id="adf14-135">$skip</span></span>           |<span data-ttu-id="adf14-136">int</span><span class="sxs-lookup"><span data-stu-id="adf14-136">int</span></span>      |<span data-ttu-id="adf14-137">Пропустить первые n результаты, полезные для paging.</span><span class="sxs-lookup"><span data-stu-id="adf14-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="adf14-138">$top</span><span class="sxs-lookup"><span data-stu-id="adf14-138">$top</span></span>            |<span data-ttu-id="adf14-139">int</span><span class="sxs-lookup"><span data-stu-id="adf14-139">int</span></span>      |<span data-ttu-id="adf14-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="adf14-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="adf14-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="adf14-141">Request headers</span></span>

| <span data-ttu-id="adf14-142">Имя</span><span class="sxs-lookup"><span data-stu-id="adf14-142">Name</span></span>           |<span data-ttu-id="adf14-143">Описание</span><span class="sxs-lookup"><span data-stu-id="adf14-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="adf14-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="adf14-144">Authorization</span></span>  | <span data-ttu-id="adf14-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adf14-p105">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="adf14-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adf14-147">Request body</span></span>

<span data-ttu-id="adf14-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="adf14-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adf14-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="adf14-149">Response</span></span>

<span data-ttu-id="adf14-150">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов personInterest](../resources/personinterest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="adf14-150">If successful, this method returns a `200 OK` response code and a collection of [personInterest](../resources/personinterest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adf14-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="adf14-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="adf14-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="adf14-152">Request</span></span>

<span data-ttu-id="adf14-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adf14-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adf14-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="adf14-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_interests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/interests
```
# <a name="c"></a>[<span data-ttu-id="adf14-155">C#</span><span class="sxs-lookup"><span data-stu-id="adf14-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adf14-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adf14-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adf14-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adf14-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adf14-158">Java</span><span class="sxs-lookup"><span data-stu-id="adf14-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-interests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="adf14-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="adf14-159">Response</span></span>

<span data-ttu-id="adf14-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="adf14-160">The following is an example of the response.</span></span>

> <span data-ttu-id="adf14-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="adf14-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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


