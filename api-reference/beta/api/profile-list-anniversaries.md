---
title: Список юбилеев
description: Получение списка объектов персонанниверсари.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2da148080d519e6be25b1d8c8bc787061e73f579
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455216"
---
# <a name="list-anniversaries"></a><span data-ttu-id="796bc-103">Список юбилеев</span><span class="sxs-lookup"><span data-stu-id="796bc-103">List anniversaries</span></span>

<span data-ttu-id="796bc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="796bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="796bc-105">Получает список объектов [персонанниверсари](../resources/personanniversary.md) для определенного пользователя из своего [профиля](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="796bc-105">Retrieves a list of the [personAnniversary](../resources/personanniversary.md) objects for the given user from their [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="796bc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="796bc-106">Permissions</span></span>

<span data-ttu-id="796bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="796bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="796bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="796bc-109">Permission type</span></span>                        | <span data-ttu-id="796bc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="796bc-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="796bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="796bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="796bc-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="796bc-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="796bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="796bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="796bc-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="796bc-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="796bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="796bc-115">Application</span></span>                            | <span data-ttu-id="796bc-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="796bc-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="796bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="796bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/anniversaries 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="796bc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="796bc-118">Optional query parameters</span></span>

<span data-ttu-id="796bc-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="796bc-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="796bc-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="796bc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="796bc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="796bc-121">Name</span></span>            |<span data-ttu-id="796bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="796bc-122">Value</span></span>    |<span data-ttu-id="796bc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="796bc-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="796bc-124">$filter</span><span class="sxs-lookup"><span data-stu-id="796bc-124">$filter</span></span>         |<span data-ttu-id="796bc-125">string</span><span class="sxs-lookup"><span data-stu-id="796bc-125">string</span></span>   |<span data-ttu-id="796bc-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="796bc-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="796bc-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="796bc-127">$orderby</span></span>        |<span data-ttu-id="796bc-128">строка</span><span class="sxs-lookup"><span data-stu-id="796bc-128">string</span></span>   |<span data-ttu-id="796bc-129">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="796bc-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="796bc-130">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="796bc-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="796bc-131">$select</span><span class="sxs-lookup"><span data-stu-id="796bc-131">$select</span></span>         |<span data-ttu-id="796bc-132">string</span><span class="sxs-lookup"><span data-stu-id="796bc-132">string</span></span>   |<span data-ttu-id="796bc-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="796bc-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="796bc-135">$skip</span><span class="sxs-lookup"><span data-stu-id="796bc-135">$skip</span></span>           |<span data-ttu-id="796bc-136">int</span><span class="sxs-lookup"><span data-stu-id="796bc-136">int</span></span>      |<span data-ttu-id="796bc-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="796bc-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="796bc-138">$top</span><span class="sxs-lookup"><span data-stu-id="796bc-138">$top</span></span>            |<span data-ttu-id="796bc-139">int</span><span class="sxs-lookup"><span data-stu-id="796bc-139">int</span></span>      |<span data-ttu-id="796bc-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="796bc-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="796bc-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="796bc-141">Request headers</span></span>

| <span data-ttu-id="796bc-142">Имя</span><span class="sxs-lookup"><span data-stu-id="796bc-142">Name</span></span>           |<span data-ttu-id="796bc-143">Описание</span><span class="sxs-lookup"><span data-stu-id="796bc-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="796bc-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="796bc-144">Authorization</span></span>  | <span data-ttu-id="796bc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="796bc-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="796bc-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="796bc-147">Request body</span></span>

<span data-ttu-id="796bc-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="796bc-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="796bc-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="796bc-149">Response</span></span>

<span data-ttu-id="796bc-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [персонанниверсари](../resources/personanniversary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="796bc-150">If successful, this method returns a `200 OK` response code and a collection of [personAnniversary](../resources/personanniversary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="796bc-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="796bc-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="796bc-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="796bc-152">Request</span></span>

<span data-ttu-id="796bc-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="796bc-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="796bc-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="796bc-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_anniversaries"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/anniversaries
```
# <a name="c"></a>[<span data-ttu-id="796bc-155">C#</span><span class="sxs-lookup"><span data-stu-id="796bc-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-anniversaries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="796bc-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="796bc-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-anniversaries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="796bc-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="796bc-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-anniversaries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="796bc-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="796bc-158">Response</span></span>

<span data-ttu-id="796bc-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="796bc-159">The following is an example of the response.</span></span>

> <span data-ttu-id="796bc-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="796bc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "type": "type-value",
      "date": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List anniversaries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
