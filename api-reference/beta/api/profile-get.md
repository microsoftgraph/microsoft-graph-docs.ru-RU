---
title: Получение профиля
description: Извлечение свойств и связей объекта профиля.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8a9eab6e17da201e7a63dfb79e290ceca8f79fa6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049851"
---
# <a name="get-profile"></a><span data-ttu-id="74c15-103">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="74c15-103">Get profile</span></span>

<span data-ttu-id="74c15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74c15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74c15-105">Извлечение свойств и связей объекта [профиля](../resources/profile.md) для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="74c15-105">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

<span data-ttu-id="74c15-106">Ресурс **профиля** предоставляет различные богатые свойства, описательные для пользователя, как [отношения,](../resources/profile.md#relationships)например, юбилеи и образовательные мероприятия.</span><span class="sxs-lookup"><span data-stu-id="74c15-106">The **profile** resource exposes various rich properties that are descriptive of the user as [relationships](../resources/profile.md#relationships), for example, anniversaries and education activities.</span></span> <span data-ttu-id="74c15-107">Чтобы получить одно из этих свойств навигации, используйте соответствующий метод GET в этом свойстве.</span><span class="sxs-lookup"><span data-stu-id="74c15-107">To get one of these navigation properties, use the corresponding GET method on that property.</span></span> <span data-ttu-id="74c15-108">См. [методы,](../resources/profile.md) открытые **профилем**.</span><span class="sxs-lookup"><span data-stu-id="74c15-108">See the [methods](../resources/profile.md) exposed by **profile**.</span></span>

## <a name="permissions"></a><span data-ttu-id="74c15-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74c15-109">Permissions</span></span>

<span data-ttu-id="74c15-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74c15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74c15-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74c15-112">Permission type</span></span>                        | <span data-ttu-id="74c15-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74c15-113">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="74c15-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74c15-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="74c15-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c15-115">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="74c15-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74c15-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c15-117">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c15-117">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="74c15-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="74c15-118">Application</span></span>                            | <span data-ttu-id="74c15-119">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c15-119">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="74c15-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74c15-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
GET /users/{id | userPrincipalName}/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74c15-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="74c15-121">Optional query parameters</span></span>

<span data-ttu-id="74c15-122">Этот метод поддерживает параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="74c15-122">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="74c15-123">Укажите список свойств, которые необходимо включить в ответ, разделив их запятой.</span><span class="sxs-lookup"><span data-stu-id="74c15-123">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="74c15-124">Для оптимальной производительности выберите только подмножество необходимых свойств.</span><span class="sxs-lookup"><span data-stu-id="74c15-124">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74c15-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74c15-125">Request headers</span></span>

| <span data-ttu-id="74c15-126">Имя</span><span class="sxs-lookup"><span data-stu-id="74c15-126">Name</span></span>           |<span data-ttu-id="74c15-127">Описание</span><span class="sxs-lookup"><span data-stu-id="74c15-127">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="74c15-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74c15-128">Authorization</span></span>  | <span data-ttu-id="74c15-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74c15-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="74c15-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74c15-131">Content-Type</span></span>   | <span data-ttu-id="74c15-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74c15-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74c15-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74c15-134">Request body</span></span>

<span data-ttu-id="74c15-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74c15-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74c15-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="74c15-136">Response</span></span>

<span data-ttu-id="74c15-137">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` профиля в тексте ответа. [](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="74c15-137">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74c15-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="74c15-138">Examples</span></span>

### <a name="example-1-get-a-users-profile"></a><span data-ttu-id="74c15-139">Пример 1. Получить профиль пользователя</span><span class="sxs-lookup"><span data-stu-id="74c15-139">Example 1: GET a user's profile</span></span>

<span data-ttu-id="74c15-140">Ниже приводится пример запроса на профиль GET.</span><span class="sxs-lookup"><span data-stu-id="74c15-140">The following is an example of the GET profile request.</span></span>

#### <a name="request"></a><span data-ttu-id="74c15-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="74c15-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="74c15-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="74c15-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="74c15-143">C#</span><span class="sxs-lookup"><span data-stu-id="74c15-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74c15-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74c15-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74c15-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74c15-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74c15-146">Java</span><span class="sxs-lookup"><span data-stu-id="74c15-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profile-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="74c15-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="74c15-147">Response</span></span>

<span data-ttu-id="74c15-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="74c15-148">The following is an example of the response.</span></span>

> <span data-ttu-id="74c15-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="74c15-149">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "34545-32444234-2334452-234332-432234",
  "accounts": [],
  "addresses": [
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
      "displayName": "Home",
      "detail": {
        "type": "home",
        "postOfficeBox": null,
        "street": "221B Baker Street",
        "city": "London",
        "state": null,
        "countryOrRegion": "United Kingdom",
        "postalCode": "E14 3TD"
      },
      "geoCoordinates": null
    }
  ],
  "anniversaries": [
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
      "type": "birthday",
      "date": "Date"
    }
  ],
  "websites": [],
  "educationalActivities": [],
  "emails": [
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
  ],
  "notes": [],
  "interests": [],
  "languages": [],
  "names": [
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
      "displayName": "Innocenty Popov",
      "first": "Innocenty",
      "initials": "IP",
      "last": "Popov",
      "languageTag": "en-US",
      "maiden": null,
      "middle": null,
      "nickname": "Kesha",
      "suffix": null,
      "title": null,
      "pronunciation": {
        "displayName": "In-no ken-te ",
        "first": "In-no ken-te Pop-ov",
        "maiden": null,
        "middle": null,
        "last": "Pop-ov"
      }
    }
  ],
  "phones": [
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
  ],
  "positions": [],
  "projects": [],
  "skills": [],
  "webAccounts": []
}
```

### <a name="example-2-expand-names-and-skills-collection-and-select-properties-within-the-entities"></a><span data-ttu-id="74c15-150">Пример 2. Расширение коллекции имен и навыков и выбор свойств в сущностями</span><span class="sxs-lookup"><span data-stu-id="74c15-150">Example 2: Expand names and skills collection and select properties within the entities</span></span>

<span data-ttu-id="74c15-151">Ниже приводится пример использования параметров $expand и $select для получения частичной информации из профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="74c15-151">The following is an example of using the $expand and $select query parameters to retrieve partial information from a user's profile.</span></span>

#### <a name="request"></a><span data-ttu-id="74c15-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="74c15-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="74c15-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="74c15-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile?$expand=names($select=first,last),skills($select=displayName)
```
# <a name="c"></a>[<span data-ttu-id="74c15-154">C#</span><span class="sxs-lookup"><span data-stu-id="74c15-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74c15-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74c15-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74c15-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74c15-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74c15-157">Java</span><span class="sxs-lookup"><span data-stu-id="74c15-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profile-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="74c15-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="74c15-158">Response</span></span>

<span data-ttu-id="74c15-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="74c15-159">The following is an example of the response.</span></span>

> <span data-ttu-id="74c15-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="74c15-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "34545-32444234-2334452-234332-432234",
  "names": [
      {
          "first": "Innocenty",
          "last": "Popov"
      }
  ],
  "skills": [
      {
          "displayName": "Machine Learning"
      },
      {
          "displayName": "Artificial Intelligence"
      }
  ]
}
```


