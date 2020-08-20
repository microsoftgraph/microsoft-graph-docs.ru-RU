---
title: Список сообщений электронной почты
description: Получение списка объектов itemEmail.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a3ab4f80069131904d9d619e7ddddb72c5a19511
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819471"
---
# <a name="list-emails"></a><span data-ttu-id="48816-103">Список сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="48816-103">List emails</span></span>

<span data-ttu-id="48816-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48816-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48816-105">Получение списка [объектов itemEmail](../resources/itememail.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="48816-105">Retrieve a list of [itemEmail](../resources/itememail.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48816-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48816-106">Permissions</span></span>

<span data-ttu-id="48816-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48816-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48816-109">Permission type</span></span>                        | <span data-ttu-id="48816-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48816-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="48816-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48816-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48816-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48816-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="48816-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48816-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48816-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48816-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="48816-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="48816-115">Application</span></span>                            | <span data-ttu-id="48816-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48816-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48816-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48816-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/emails
GET /users/{id | userPrincipalName}/profile/emails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48816-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48816-118">Optional query parameters</span></span>

<span data-ttu-id="48816-119">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="48816-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="48816-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="48816-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="48816-121">Имя</span><span class="sxs-lookup"><span data-stu-id="48816-121">Name</span></span>            |<span data-ttu-id="48816-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48816-122">Value</span></span>    |<span data-ttu-id="48816-123">Описание</span><span class="sxs-lookup"><span data-stu-id="48816-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="48816-124">$filter</span><span class="sxs-lookup"><span data-stu-id="48816-124">$filter</span></span>         |<span data-ttu-id="48816-125">string</span><span class="sxs-lookup"><span data-stu-id="48816-125">string</span></span>   |<span data-ttu-id="48816-126">Возвращает число в отклике только тех объектов, которые содержат указанные условия.</span><span class="sxs-lookup"><span data-stu-id="48816-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="48816-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="48816-127">$orderby</span></span>        |<span data-ttu-id="48816-128">строка</span><span class="sxs-lookup"><span data-stu-id="48816-128">string</span></span>   |<span data-ttu-id="48816-129">По умолчанию объекты в ответе сортируются по их значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="48816-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="48816-130">Этот порядок ответа можно изменить с помощью *$orderby* параметра.</span><span class="sxs-lookup"><span data-stu-id="48816-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="48816-131">$select</span><span class="sxs-lookup"><span data-stu-id="48816-131">$select</span></span>         |<span data-ttu-id="48816-132">string</span><span class="sxs-lookup"><span data-stu-id="48816-132">string</span></span>   |<span data-ttu-id="48816-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="48816-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="48816-135">$skip</span><span class="sxs-lookup"><span data-stu-id="48816-135">$skip</span></span>           |<span data-ttu-id="48816-136">int</span><span class="sxs-lookup"><span data-stu-id="48816-136">int</span></span>      |<span data-ttu-id="48816-137">Пропуск первых n результатов; это удобно при разбиении результатов на страницы.</span><span class="sxs-lookup"><span data-stu-id="48816-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="48816-138">$top</span><span class="sxs-lookup"><span data-stu-id="48816-138">$top</span></span>            |<span data-ttu-id="48816-139">int</span><span class="sxs-lookup"><span data-stu-id="48816-139">int</span></span>      |<span data-ttu-id="48816-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="48816-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="48816-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="48816-141">Request headers</span></span>

| <span data-ttu-id="48816-142">Имя</span><span class="sxs-lookup"><span data-stu-id="48816-142">Name</span></span>           |<span data-ttu-id="48816-143">Описание</span><span class="sxs-lookup"><span data-stu-id="48816-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="48816-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48816-144">Authorization</span></span>  | <span data-ttu-id="48816-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48816-p105">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="48816-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48816-147">Request body</span></span>
<span data-ttu-id="48816-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48816-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48816-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="48816-149">Response</span></span>

<span data-ttu-id="48816-150">При успешном выполнении этот метод возвращает `200 OK` код отклика и коллекцию объектов [itemEmail в](../resources/itememail.md) тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48816-150">If successful, this method returns a `200 OK` response code and a collection of [itemEmail](../resources/itememail.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48816-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="48816-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="48816-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="48816-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emails"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/emails
```
# <a name="c"></a>[<span data-ttu-id="48816-153">C#</span><span class="sxs-lookup"><span data-stu-id="48816-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48816-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48816-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48816-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48816-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="48816-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="48816-156">Response</span></span>

<span data-ttu-id="48816-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="48816-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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
