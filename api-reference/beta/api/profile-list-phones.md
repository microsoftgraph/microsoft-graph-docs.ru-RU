---
title: Телефоны списка
description: Извлечение списка объектов itemPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f8034647c80e334e96066afdcf6f44d4cb129dd0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950584"
---
# <a name="list-phones"></a><span data-ttu-id="623a5-103">Телефоны списка</span><span class="sxs-lookup"><span data-stu-id="623a5-103">List phones</span></span>

<span data-ttu-id="623a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="623a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="623a5-105">Извлечение списка [объектов itemPhone](../resources/itemphone.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="623a5-105">Retrieve a list of [itemPhone](../resources/itemphone.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="623a5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="623a5-106">Permissions</span></span>

<span data-ttu-id="623a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="623a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="623a5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="623a5-109">Permission type</span></span>                        | <span data-ttu-id="623a5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="623a5-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="623a5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="623a5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="623a5-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623a5-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="623a5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="623a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="623a5-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623a5-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="623a5-115">Application</span><span class="sxs-lookup"><span data-stu-id="623a5-115">Application</span></span>                            | <span data-ttu-id="623a5-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623a5-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="623a5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="623a5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/phones
GET /users/{id | userPrincipalName}/profile/phones
```

## <a name="optional-query-parameters"></a><span data-ttu-id="623a5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="623a5-118">Optional query parameters</span></span>

<span data-ttu-id="623a5-119">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="623a5-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="623a5-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="623a5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="623a5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="623a5-121">Name</span></span>            |<span data-ttu-id="623a5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="623a5-122">Value</span></span>    |<span data-ttu-id="623a5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="623a5-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="623a5-124">$filter</span><span class="sxs-lookup"><span data-stu-id="623a5-124">$filter</span></span>         |<span data-ttu-id="623a5-125">string</span><span class="sxs-lookup"><span data-stu-id="623a5-125">string</span></span>   |<span data-ttu-id="623a5-126">Ограничивает ответ только теми объектами, которые содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="623a5-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="623a5-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="623a5-127">$orderby</span></span>        |<span data-ttu-id="623a5-128">строка</span><span class="sxs-lookup"><span data-stu-id="623a5-128">string</span></span>   |<span data-ttu-id="623a5-129">По умолчанию объекты в ответе сортируют по их созданному значениюDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="623a5-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="623a5-130">Вы можете изменить порядок ответа с помощью *параметра $orderby.*</span><span class="sxs-lookup"><span data-stu-id="623a5-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="623a5-131">$select</span><span class="sxs-lookup"><span data-stu-id="623a5-131">$select</span></span>         |<span data-ttu-id="623a5-132">string</span><span class="sxs-lookup"><span data-stu-id="623a5-132">string</span></span>   |<span data-ttu-id="623a5-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="623a5-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="623a5-135">$skip</span><span class="sxs-lookup"><span data-stu-id="623a5-135">$skip</span></span>           |<span data-ttu-id="623a5-136">int</span><span class="sxs-lookup"><span data-stu-id="623a5-136">int</span></span>      |<span data-ttu-id="623a5-137">Пропустить первые n результаты, полезные для paging.</span><span class="sxs-lookup"><span data-stu-id="623a5-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="623a5-138">$top</span><span class="sxs-lookup"><span data-stu-id="623a5-138">$top</span></span>            |<span data-ttu-id="623a5-139">int</span><span class="sxs-lookup"><span data-stu-id="623a5-139">int</span></span>      |<span data-ttu-id="623a5-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="623a5-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="623a5-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="623a5-141">Request headers</span></span>

|<span data-ttu-id="623a5-142">Имя</span><span class="sxs-lookup"><span data-stu-id="623a5-142">Name</span></span>|<span data-ttu-id="623a5-143">Описание</span><span class="sxs-lookup"><span data-stu-id="623a5-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="623a5-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="623a5-144">Authorization</span></span>|<span data-ttu-id="623a5-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="623a5-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="623a5-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="623a5-147">Request body</span></span>

<span data-ttu-id="623a5-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="623a5-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="623a5-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="623a5-149">Response</span></span>

<span data-ttu-id="623a5-150">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [itemPhone](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="623a5-150">If successful, this method returns a `200 OK` response code and a collection of [itemPhone](../resources/itemphone.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="623a5-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="623a5-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="623a5-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="623a5-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="623a5-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="623a5-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemphone_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/me/profile/phones
```
# <a name="c"></a>[<span data-ttu-id="623a5-154">C#</span><span class="sxs-lookup"><span data-stu-id="623a5-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemphone-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="623a5-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="623a5-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemphone-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="623a5-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="623a5-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemphone-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="623a5-157">Java</span><span class="sxs-lookup"><span data-stu-id="623a5-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-itemphone-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="623a5-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="623a5-158">Response</span></span>
<span data-ttu-id="623a5-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="623a5-159">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemPhone)"
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
      "displayName": "Car Phone",
      "type": "other",
      "number": "+7 499 342 22 13"
    }
  ]
}
```


