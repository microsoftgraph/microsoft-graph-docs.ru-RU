---
title: Список сообщений электронной почты
description: Получение списка объектов Итемемаил.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 89712a37f289c855d5a09510ca0c9b9b6495bf60
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980839"
---
# <a name="list-emails"></a><span data-ttu-id="4b112-103">Список сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="4b112-103">List emails</span></span>

<span data-ttu-id="4b112-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b112-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b112-105">Получение списка объектов [итемемаил](../resources/itememail.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="4b112-105">Retrieve a list of [itemEmail](../resources/itememail.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b112-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b112-106">Permissions</span></span>

<span data-ttu-id="4b112-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b112-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b112-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b112-109">Permission type</span></span>                        | <span data-ttu-id="4b112-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b112-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b112-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b112-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b112-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4b112-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4b112-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b112-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b112-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4b112-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4b112-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4b112-115">Application</span></span>                            | <span data-ttu-id="4b112-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4b112-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b112-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b112-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/emails
GET /users/{id | userPrincipalName}/profile/emails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b112-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4b112-118">Optional query parameters</span></span>

<span data-ttu-id="4b112-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4b112-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="4b112-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4b112-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="4b112-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4b112-121">Name</span></span>            |<span data-ttu-id="4b112-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b112-122">Value</span></span>    |<span data-ttu-id="4b112-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4b112-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4b112-124">$filter</span><span class="sxs-lookup"><span data-stu-id="4b112-124">$filter</span></span>         |<span data-ttu-id="4b112-125">string</span><span class="sxs-lookup"><span data-stu-id="4b112-125">string</span></span>   |<span data-ttu-id="4b112-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="4b112-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="4b112-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="4b112-127">$orderby</span></span>        |<span data-ttu-id="4b112-128">строка</span><span class="sxs-lookup"><span data-stu-id="4b112-128">string</span></span>   |<span data-ttu-id="4b112-129">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="4b112-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="4b112-130">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="4b112-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="4b112-131">$select</span><span class="sxs-lookup"><span data-stu-id="4b112-131">$select</span></span>         |<span data-ttu-id="4b112-132">string</span><span class="sxs-lookup"><span data-stu-id="4b112-132">string</span></span>   |<span data-ttu-id="4b112-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="4b112-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="4b112-135">$skip</span><span class="sxs-lookup"><span data-stu-id="4b112-135">$skip</span></span>           |<span data-ttu-id="4b112-136">int</span><span class="sxs-lookup"><span data-stu-id="4b112-136">int</span></span>      |<span data-ttu-id="4b112-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="4b112-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="4b112-138">$top</span><span class="sxs-lookup"><span data-stu-id="4b112-138">$top</span></span>            |<span data-ttu-id="4b112-139">int</span><span class="sxs-lookup"><span data-stu-id="4b112-139">int</span></span>      |<span data-ttu-id="4b112-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="4b112-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="4b112-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b112-141">Request headers</span></span>

| <span data-ttu-id="4b112-142">Имя</span><span class="sxs-lookup"><span data-stu-id="4b112-142">Name</span></span>           |<span data-ttu-id="4b112-143">Описание</span><span class="sxs-lookup"><span data-stu-id="4b112-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4b112-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b112-144">Authorization</span></span>  | <span data-ttu-id="4b112-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b112-p105">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="4b112-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b112-147">Request body</span></span>
<span data-ttu-id="4b112-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b112-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b112-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b112-149">Response</span></span>

<span data-ttu-id="4b112-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [итемемаил](../resources/itememail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b112-150">If successful, this method returns a `200 OK` response code and a collection of [itemEmail](../resources/itememail.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b112-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="4b112-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="4b112-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b112-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emails"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/emails
```
# <a name="c"></a>[<span data-ttu-id="4b112-153">C#</span><span class="sxs-lookup"><span data-stu-id="4b112-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b112-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b112-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b112-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b112-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b112-156">Java</span><span class="sxs-lookup"><span data-stu-id="4b112-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4b112-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b112-157">Response</span></span>

<span data-ttu-id="4b112-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4b112-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "e13f7a4d-303c-464f-a6af-80ea18eb74f3",
      "allowedAudiences": "organization",
      "inference": null,
      "createdDateTime": "2020-07-06T06:34:12.2294868Z",
      "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Innocenty Popov"
        }
      },
      "lastModifiedDateTime": "2020-07-08T06:34:12.2294868Z",
      "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Innocenty Popov"
        }
      },
      "source": {
        "type": "User"
      },
      "address": "innocenty.popov@adventureworks.com",
      "displayName": "Innocenty Popov",
      "type": "work"
    }
  ]
}
```


