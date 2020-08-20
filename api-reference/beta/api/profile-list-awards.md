---
title: Список набиратей
description: Получение коллекции personAwards из свойства навигации с набое.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2b2315a037b6f8e04ec420955ffee591029a81a5
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819328"
---
# <a name="list-awards"></a><span data-ttu-id="f9c23-103">Список набиратей</span><span class="sxs-lookup"><span data-stu-id="f9c23-103">List awards</span></span>

<span data-ttu-id="f9c23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9c23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9c23-105">Получение списка [объектов personAward](../resources/personaward.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="f9c23-105">Retrieve a list of [personAward](../resources/personaward.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9c23-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9c23-106">Permissions</span></span>

<span data-ttu-id="f9c23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9c23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9c23-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9c23-109">Permission type</span></span>                        | <span data-ttu-id="f9c23-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9c23-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f9c23-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9c23-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9c23-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c23-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f9c23-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9c23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9c23-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c23-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f9c23-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f9c23-115">Application</span></span>                            | <span data-ttu-id="f9c23-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c23-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f9c23-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9c23-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/awards
GET /users/{id | userPrincipalName}/profile/awards
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9c23-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9c23-118">Optional query parameters</span></span>

<span data-ttu-id="f9c23-119">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f9c23-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="f9c23-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f9c23-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="f9c23-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f9c23-121">Name</span></span>            |<span data-ttu-id="f9c23-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9c23-122">Value</span></span>    |<span data-ttu-id="f9c23-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f9c23-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="f9c23-124">$filter</span><span class="sxs-lookup"><span data-stu-id="f9c23-124">$filter</span></span>         |<span data-ttu-id="f9c23-125">string</span><span class="sxs-lookup"><span data-stu-id="f9c23-125">string</span></span>   |<span data-ttu-id="f9c23-126">Возвращает число в отклике только тех объектов, которые содержат указанные условия.</span><span class="sxs-lookup"><span data-stu-id="f9c23-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="f9c23-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="f9c23-127">$orderby</span></span>        |<span data-ttu-id="f9c23-128">строка</span><span class="sxs-lookup"><span data-stu-id="f9c23-128">string</span></span>   |<span data-ttu-id="f9c23-129">По умолчанию объекты в ответе сортируются по их значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="f9c23-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="f9c23-130">Этот порядок ответа можно изменить с помощью *$orderby* параметра.</span><span class="sxs-lookup"><span data-stu-id="f9c23-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="f9c23-131">$select</span><span class="sxs-lookup"><span data-stu-id="f9c23-131">$select</span></span>         |<span data-ttu-id="f9c23-132">string</span><span class="sxs-lookup"><span data-stu-id="f9c23-132">string</span></span>   |<span data-ttu-id="f9c23-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="f9c23-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="f9c23-135">$skip</span><span class="sxs-lookup"><span data-stu-id="f9c23-135">$skip</span></span>           |<span data-ttu-id="f9c23-136">int</span><span class="sxs-lookup"><span data-stu-id="f9c23-136">int</span></span>      |<span data-ttu-id="f9c23-137">Пропуск первых n результатов; это удобно при разбиении результатов на страницы.</span><span class="sxs-lookup"><span data-stu-id="f9c23-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="f9c23-138">$top</span><span class="sxs-lookup"><span data-stu-id="f9c23-138">$top</span></span>            |<span data-ttu-id="f9c23-139">int</span><span class="sxs-lookup"><span data-stu-id="f9c23-139">int</span></span>      |<span data-ttu-id="f9c23-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="f9c23-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="f9c23-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f9c23-141">Request headers</span></span>
|<span data-ttu-id="f9c23-142">Имя</span><span class="sxs-lookup"><span data-stu-id="f9c23-142">Name</span></span>|<span data-ttu-id="f9c23-143">Описание</span><span class="sxs-lookup"><span data-stu-id="f9c23-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f9c23-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9c23-144">Authorization</span></span>|<span data-ttu-id="f9c23-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9c23-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9c23-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9c23-147">Request body</span></span>
<span data-ttu-id="f9c23-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9c23-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9c23-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9c23-149">Response</span></span>

<span data-ttu-id="f9c23-150">При успешном выполнении этот метод возвращает `200 OK` код отклика и коллекцию [объектов personAward](../resources/personaward.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9c23-150">If successful, this method returns a `200 OK` response code and a collection of [personAward](../resources/personaward.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9c23-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="f9c23-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="f9c23-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9c23-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemawards_from_profile"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/awards
```
# <a name="c"></a>[<span data-ttu-id="f9c23-153">C#</span><span class="sxs-lookup"><span data-stu-id="f9c23-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemawards-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9c23-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9c23-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemawards-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9c23-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9c23-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemawards-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f9c23-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9c23-156">Response</span></span>
<span data-ttu-id="f9c23-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f9c23-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.personAward)"
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
      "description": "Lifetime Achievement award from the International Association of Branding Managers",
      "displayName": "Lifetime Achievement Award For Excellence in Branding",
      "issuedDate": "Date",
      "issuingAuthority": "International Association of Branding Management",
      "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
      "webUrl": "https://www.iabm.io"
    }
  ]
}
```
