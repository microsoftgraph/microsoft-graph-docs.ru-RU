---
title: Список учетных записей
description: Получение списка объектов учетных записей учетных записей.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 75d45c0dff4828c292887e7d7fb1d8a6817c53dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455167"
---
# <a name="list-webaccounts"></a><span data-ttu-id="7506b-103">Список учетных записей</span><span class="sxs-lookup"><span data-stu-id="7506b-103">List webAccounts</span></span>

<span data-ttu-id="7506b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7506b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7506b-105">Получение списка объектов [учетных записей для учетных записей](../resources/webaccount.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="7506b-105">Retrieve a list of [webAccounts](../resources/webaccount.md) objects from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7506b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7506b-106">Permissions</span></span>

<span data-ttu-id="7506b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7506b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7506b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7506b-109">Permission type</span></span>                        | <span data-ttu-id="7506b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7506b-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="7506b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7506b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7506b-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7506b-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7506b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7506b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7506b-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7506b-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7506b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7506b-115">Application</span></span>                            | <span data-ttu-id="7506b-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7506b-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="7506b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7506b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/webAccounts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7506b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7506b-118">Optional query parameters</span></span>

<span data-ttu-id="7506b-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7506b-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="7506b-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7506b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="7506b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7506b-121">Name</span></span>            |<span data-ttu-id="7506b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7506b-122">Value</span></span>    |<span data-ttu-id="7506b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7506b-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="7506b-124">$filter</span><span class="sxs-lookup"><span data-stu-id="7506b-124">$filter</span></span>         |<span data-ttu-id="7506b-125">string</span><span class="sxs-lookup"><span data-stu-id="7506b-125">string</span></span>   |<span data-ttu-id="7506b-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="7506b-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="7506b-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="7506b-127">$orderby</span></span>        |<span data-ttu-id="7506b-128">строка</span><span class="sxs-lookup"><span data-stu-id="7506b-128">string</span></span>   |<span data-ttu-id="7506b-129">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="7506b-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="7506b-130">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="7506b-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="7506b-131">$select</span><span class="sxs-lookup"><span data-stu-id="7506b-131">$select</span></span>         |<span data-ttu-id="7506b-132">string</span><span class="sxs-lookup"><span data-stu-id="7506b-132">string</span></span>   |<span data-ttu-id="7506b-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="7506b-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="7506b-135">$skip</span><span class="sxs-lookup"><span data-stu-id="7506b-135">$skip</span></span>           |<span data-ttu-id="7506b-136">int</span><span class="sxs-lookup"><span data-stu-id="7506b-136">int</span></span>      |<span data-ttu-id="7506b-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="7506b-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="7506b-138">$top</span><span class="sxs-lookup"><span data-stu-id="7506b-138">$top</span></span>            |<span data-ttu-id="7506b-139">int</span><span class="sxs-lookup"><span data-stu-id="7506b-139">int</span></span>      |<span data-ttu-id="7506b-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="7506b-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="7506b-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7506b-141">Request headers</span></span>

| <span data-ttu-id="7506b-142">Имя</span><span class="sxs-lookup"><span data-stu-id="7506b-142">Name</span></span>           |<span data-ttu-id="7506b-143">Описание</span><span class="sxs-lookup"><span data-stu-id="7506b-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="7506b-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7506b-144">Authorization</span></span>  | <span data-ttu-id="7506b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7506b-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="7506b-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7506b-147">Request body</span></span>

<span data-ttu-id="7506b-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7506b-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7506b-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="7506b-149">Response</span></span>

<span data-ttu-id="7506b-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Account](../resources/webaccount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7506b-150">If successful, this method returns a `200 OK` response code and a collection of [webAccount](../resources/webaccount.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7506b-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="7506b-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7506b-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="7506b-152">Request</span></span>

<span data-ttu-id="7506b-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7506b-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7506b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="7506b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_webaccounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/webAccounts
```
# <a name="c"></a>[<span data-ttu-id="7506b-155">C#</span><span class="sxs-lookup"><span data-stu-id="7506b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-webaccounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7506b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7506b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-webaccounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7506b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7506b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-webaccounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7506b-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="7506b-158">Response</span></span>

<span data-ttu-id="7506b-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7506b-159">The following is an example of the response.</span></span>

> <span data-ttu-id="7506b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7506b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "userId": "userId-value",
      "service": {
        "name": "name-value",
        "webUrl": "webUrl-value"
      },
      "statusMessage": "statusMessage-value",
      "webUrl": "webUrl-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List webAccounts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
