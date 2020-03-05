---
title: Получение personName
description: Получение свойств и связей объекта personName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8258abf0b39163ecce62ac601f52f8cbcec42004
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455895"
---
# <a name="get-personname"></a><span data-ttu-id="b6148-103">Получение personName</span><span class="sxs-lookup"><span data-stu-id="b6148-103">Get personName</span></span>

<span data-ttu-id="b6148-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6148-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6148-105">Получение свойств и связей объекта [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6148-105">Retrieve the properties and relationships of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6148-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6148-106">Permissions</span></span>

<span data-ttu-id="b6148-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6148-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6148-109">Permission type</span></span>                        | <span data-ttu-id="b6148-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6148-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b6148-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6148-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6148-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b6148-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b6148-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6148-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6148-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b6148-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b6148-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6148-115">Application</span></span>                            | <span data-ttu-id="b6148-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b6148-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b6148-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6148-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6148-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b6148-118">Optional query parameters</span></span>

<span data-ttu-id="b6148-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b6148-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="b6148-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b6148-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="b6148-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b6148-121">Name</span></span>            |<span data-ttu-id="b6148-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6148-122">Value</span></span>    |<span data-ttu-id="b6148-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b6148-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b6148-124">$filter</span><span class="sxs-lookup"><span data-stu-id="b6148-124">$filter</span></span>         |<span data-ttu-id="b6148-125">string</span><span class="sxs-lookup"><span data-stu-id="b6148-125">string</span></span>   |<span data-ttu-id="b6148-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="b6148-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="b6148-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="b6148-127">$orderby</span></span>        |<span data-ttu-id="b6148-128">строка</span><span class="sxs-lookup"><span data-stu-id="b6148-128">string</span></span>   |<span data-ttu-id="b6148-129">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="b6148-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="b6148-130">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="b6148-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="b6148-131">$select</span><span class="sxs-lookup"><span data-stu-id="b6148-131">$select</span></span>         |<span data-ttu-id="b6148-132">string</span><span class="sxs-lookup"><span data-stu-id="b6148-132">string</span></span>   |<span data-ttu-id="b6148-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="b6148-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="b6148-135">$skip</span><span class="sxs-lookup"><span data-stu-id="b6148-135">$skip</span></span>           |<span data-ttu-id="b6148-136">int</span><span class="sxs-lookup"><span data-stu-id="b6148-136">int</span></span>      |<span data-ttu-id="b6148-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="b6148-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="b6148-138">$top</span><span class="sxs-lookup"><span data-stu-id="b6148-138">$top</span></span>            |<span data-ttu-id="b6148-139">int</span><span class="sxs-lookup"><span data-stu-id="b6148-139">int</span></span>      |<span data-ttu-id="b6148-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="b6148-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="b6148-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6148-141">Request headers</span></span>

| <span data-ttu-id="b6148-142">Имя</span><span class="sxs-lookup"><span data-stu-id="b6148-142">Name</span></span>           |<span data-ttu-id="b6148-143">Описание</span><span class="sxs-lookup"><span data-stu-id="b6148-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b6148-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6148-144">Authorization</span></span>  | <span data-ttu-id="b6148-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6148-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b6148-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6148-147">Content-Type</span></span>   | <span data-ttu-id="b6148-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6148-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6148-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6148-150">Request body</span></span>

<span data-ttu-id="b6148-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6148-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6148-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6148-152">Response</span></span>

<span data-ttu-id="b6148-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6148-153">If successful, this method returns a `200 OK` response code and the requested [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6148-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="b6148-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6148-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6148-155">Request</span></span>

<span data-ttu-id="b6148-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6148-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6148-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6148-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personname"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names/{id}
```
# <a name="c"></a>[<span data-ttu-id="b6148-158">C#</span><span class="sxs-lookup"><span data-stu-id="b6148-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6148-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6148-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6148-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6148-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b6148-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6148-161">Response</span></span>

<span data-ttu-id="b6148-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6148-162">The following is an example of the response.</span></span>

> <span data-ttu-id="b6148-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6148-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
