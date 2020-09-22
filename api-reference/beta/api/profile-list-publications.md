---
title: Список публикаций
description: Получение Итемпубликатионс из свойства навигации публикации.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: be3aacf8993182985c100217500274128f4c96a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034653"
---
# <a name="list-publications"></a><span data-ttu-id="01ffc-103">Список публикаций</span><span class="sxs-lookup"><span data-stu-id="01ffc-103">List publications</span></span>
<span data-ttu-id="01ffc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01ffc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01ffc-105">Получение списка объектов [итемпубликатион](../resources/itempublication.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="01ffc-105">Retrieve a list of [itemPublication](../resources/itempublication.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01ffc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01ffc-106">Permissions</span></span>

<span data-ttu-id="01ffc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01ffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01ffc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01ffc-109">Permission type</span></span>                        | <span data-ttu-id="01ffc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01ffc-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="01ffc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01ffc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="01ffc-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="01ffc-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="01ffc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01ffc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01ffc-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="01ffc-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="01ffc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01ffc-115">Application</span></span>                            | <span data-ttu-id="01ffc-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="01ffc-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="01ffc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01ffc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/publications
GET /users/{id | userPrincipalName}/profile/publications
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01ffc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01ffc-118">Optional query parameters</span></span>

<span data-ttu-id="01ffc-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01ffc-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="01ffc-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="01ffc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="01ffc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="01ffc-121">Name</span></span>            |<span data-ttu-id="01ffc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01ffc-122">Value</span></span>    |<span data-ttu-id="01ffc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="01ffc-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="01ffc-124">$filter</span><span class="sxs-lookup"><span data-stu-id="01ffc-124">$filter</span></span>         |<span data-ttu-id="01ffc-125">string</span><span class="sxs-lookup"><span data-stu-id="01ffc-125">string</span></span>   |<span data-ttu-id="01ffc-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="01ffc-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="01ffc-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="01ffc-127">$orderby</span></span>        |<span data-ttu-id="01ffc-128">строка</span><span class="sxs-lookup"><span data-stu-id="01ffc-128">string</span></span>   |<span data-ttu-id="01ffc-129">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="01ffc-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="01ffc-130">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="01ffc-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="01ffc-131">$select</span><span class="sxs-lookup"><span data-stu-id="01ffc-131">$select</span></span>         |<span data-ttu-id="01ffc-132">string</span><span class="sxs-lookup"><span data-stu-id="01ffc-132">string</span></span>   |<span data-ttu-id="01ffc-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="01ffc-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="01ffc-135">$skip</span><span class="sxs-lookup"><span data-stu-id="01ffc-135">$skip</span></span>           |<span data-ttu-id="01ffc-136">int</span><span class="sxs-lookup"><span data-stu-id="01ffc-136">int</span></span>      |<span data-ttu-id="01ffc-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="01ffc-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="01ffc-138">$top</span><span class="sxs-lookup"><span data-stu-id="01ffc-138">$top</span></span>            |<span data-ttu-id="01ffc-139">int</span><span class="sxs-lookup"><span data-stu-id="01ffc-139">int</span></span>      |<span data-ttu-id="01ffc-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="01ffc-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="01ffc-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01ffc-141">Request headers</span></span>
|<span data-ttu-id="01ffc-142">Имя</span><span class="sxs-lookup"><span data-stu-id="01ffc-142">Name</span></span>|<span data-ttu-id="01ffc-143">Описание</span><span class="sxs-lookup"><span data-stu-id="01ffc-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="01ffc-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01ffc-144">Authorization</span></span>|<span data-ttu-id="01ffc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01ffc-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01ffc-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01ffc-147">Request body</span></span>
<span data-ttu-id="01ffc-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01ffc-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01ffc-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="01ffc-149">Response</span></span>

<span data-ttu-id="01ffc-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [итемпубликатион](../resources/itempublication.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01ffc-150">If successful, this method returns a `200 OK` response code and a collection of [itemPublication](../resources/itempublication.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01ffc-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="01ffc-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="01ffc-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="01ffc-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publications_from_profile"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/publications
```
# <a name="c"></a>[<span data-ttu-id="01ffc-153">C#</span><span class="sxs-lookup"><span data-stu-id="01ffc-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publications-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01ffc-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01ffc-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publications-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01ffc-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01ffc-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publications-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="01ffc-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="01ffc-156">Response</span></span>
<span data-ttu-id="01ffc-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="01ffc-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemPublication)"
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
      "source": null,
      "description": "One persons journey to the top of the branding management field.",
      "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
      "publishedDate": "Date",
      "publisher": "International Association of Branding Management Publishing",
      "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
      "webUrl": "https://www.iabm.io"
    }
  ]
}
```


