---
title: Получение профиля
description: Получение свойств и связей объекта Profile.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 378626e8fb00e78a8fd01357d0b98614219fbbcf
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812851"
---
# <a name="get-profile"></a><span data-ttu-id="2c398-103">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="2c398-103">Get profile</span></span>

<span data-ttu-id="2c398-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c398-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c398-105">Получение свойств и связей объекта [Profile](../resources/profile.md) для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c398-105">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

<span data-ttu-id="2c398-106">Ресурс **Profile** предоставляет различные расширенные свойства, которые могут быть описательными для пользователя как [отношения](../resources/profile.md#relationships), например юбилеи и действия по образованию.</span><span class="sxs-lookup"><span data-stu-id="2c398-106">The **profile** resource exposes various rich properties that are descriptive of the user as [relationships](../resources/profile.md#relationships), for example, anniversaries and education activities.</span></span> <span data-ttu-id="2c398-107">Чтобы получить одно из этих свойств навигации, используйте соответствующий метод GET для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="2c398-107">To get one of these navigation properties, use the corresponding GET method on that property.</span></span> <span data-ttu-id="2c398-108">Просмотрите [методы](../resources/profile.md) , предоставляемые **профилем**.</span><span class="sxs-lookup"><span data-stu-id="2c398-108">See the [methods](../resources/profile.md) exposed by **profile**.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c398-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c398-109">Permissions</span></span>

<span data-ttu-id="2c398-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c398-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c398-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c398-112">Permission type</span></span>                        | <span data-ttu-id="2c398-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c398-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2c398-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c398-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c398-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c398-115">Not supported.</span></span>                              |
| <span data-ttu-id="2c398-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c398-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c398-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c398-117">Not supported.</span></span>                              |
| <span data-ttu-id="2c398-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c398-118">Application</span></span>                            | <span data-ttu-id="2c398-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c398-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="2c398-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c398-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
GET /users/{id | userPrincipalName}/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c398-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2c398-121">Optional query parameters</span></span>

<span data-ttu-id="2c398-122">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="2c398-122">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="2c398-123">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="2c398-123">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="2c398-124">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="2c398-124">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c398-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c398-125">Request headers</span></span>

| <span data-ttu-id="2c398-126">Имя</span><span class="sxs-lookup"><span data-stu-id="2c398-126">Name</span></span>           |<span data-ttu-id="2c398-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2c398-127">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="2c398-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c398-128">Authorization</span></span>  | <span data-ttu-id="2c398-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c398-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2c398-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c398-131">Content-Type</span></span>   | <span data-ttu-id="2c398-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c398-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c398-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c398-134">Request body</span></span>

<span data-ttu-id="2c398-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c398-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c398-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c398-136">Response</span></span>

<span data-ttu-id="2c398-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Profile](../resources/profile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c398-137">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c398-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="2c398-138">Examples</span></span>

### <a name="example-1-get-a-users-profile"></a><span data-ttu-id="2c398-139">Пример 1: получение профиля пользователя</span><span class="sxs-lookup"><span data-stu-id="2c398-139">Example 1: GET a user's profile</span></span>

<span data-ttu-id="2c398-140">Ниже приведен пример запроса на получение профиля.</span><span class="sxs-lookup"><span data-stu-id="2c398-140">The following is an example of the GET profile request.</span></span>

#### <a name="request"></a><span data-ttu-id="2c398-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c398-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2c398-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c398-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="2c398-143">C#</span><span class="sxs-lookup"><span data-stu-id="2c398-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c398-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c398-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c398-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c398-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2c398-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c398-146">Response</span></span>

<span data-ttu-id="2c398-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c398-147">The following is an example of the response.</span></span>

> <span data-ttu-id="2c398-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c398-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-expand-names-and-skills-collection-and-select-properties-within-the-entities"></a><span data-ttu-id="2c398-150">Пример 2: разверните элемент Names and Skills Collection и выберите свойства в объектах.</span><span class="sxs-lookup"><span data-stu-id="2c398-150">Example 2: Expand names and skills collection and select properties within the entities</span></span>

<span data-ttu-id="2c398-151">Ниже приведен пример использования параметров запроса $expand и $select для получения частичных сведений из профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c398-151">The following is an example of using the $expand and $select query parameters to retrieve partial information from a user's profile.</span></span>

#### <a name="request"></a><span data-ttu-id="2c398-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c398-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2c398-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c398-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile?$expand=names($select=first,last),skills($select=displayName)
```
# <a name="c"></a>[<span data-ttu-id="2c398-154">C#</span><span class="sxs-lookup"><span data-stu-id="2c398-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c398-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c398-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c398-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c398-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2c398-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c398-157">Response</span></span>

<span data-ttu-id="2c398-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c398-158">The following is an example of the response.</span></span>

> <span data-ttu-id="2c398-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c398-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
