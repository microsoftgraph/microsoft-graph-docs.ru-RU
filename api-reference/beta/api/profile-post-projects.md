---
title: Создание ПрожектпартиЦипатион
description: Используйте этот API для создания нового ПрожектпартиЦипатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 16ffd76c33cf61d6e8ad7522d6e5978b9aad37dc
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228634"
---
# <a name="create-projectparticipation"></a><span data-ttu-id="def72-103">Создание ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="def72-103">Create projectParticipation</span></span>

<span data-ttu-id="def72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="def72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="def72-105">Используйте этот API, чтобы создать новый объект [прожектпартиЦипатион](../resources/projectParticipation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="def72-105">Use this API to create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="def72-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="def72-106">Permissions</span></span>

<span data-ttu-id="def72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="def72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="def72-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="def72-109">Permission type</span></span>                        | <span data-ttu-id="def72-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="def72-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="def72-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="def72-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="def72-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="def72-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="def72-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="def72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="def72-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="def72-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="def72-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="def72-115">Application</span></span>                            | <span data-ttu-id="def72-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def72-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="def72-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="def72-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/projects
```

## <a name="request-headers"></a><span data-ttu-id="def72-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="def72-118">Request headers</span></span>

| <span data-ttu-id="def72-119">Имя</span><span class="sxs-lookup"><span data-stu-id="def72-119">Name</span></span>           |<span data-ttu-id="def72-120">Описание</span><span class="sxs-lookup"><span data-stu-id="def72-120">Description</span></span>                  |
|:---------------|:----------                  |
| <span data-ttu-id="def72-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="def72-121">Authorization</span></span>  | <span data-ttu-id="def72-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="def72-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="def72-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="def72-124">Content-Type</span></span>   | <span data-ttu-id="def72-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="def72-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="def72-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="def72-127">Request body</span></span>

<span data-ttu-id="def72-128">В тексте запроса добавьте представление объекта [прожектпартиЦипатион](../resources/projectparticipation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="def72-128">In the request body, supply a JSON representation of [projectParticipation](../resources/projectparticipation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="def72-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="def72-129">Response</span></span>

<span data-ttu-id="def72-130">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [прожектпартиЦипатион](../resources/projectparticipation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="def72-130">If successful, this method returns `201, Created` response code and a new [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="def72-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="def72-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="def72-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="def72-132">Request</span></span>

<span data-ttu-id="def72-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="def72-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="def72-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="def72-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_projectparticipation_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/projects
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="def72-135">C#</span><span class="sxs-lookup"><span data-stu-id="def72-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-projectparticipation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="def72-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="def72-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-projectparticipation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="def72-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="def72-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-projectparticipation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="def72-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="def72-138">Response</span></span>

<span data-ttu-id="def72-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="def72-139">The following is an example of the response.</span></span>

> <span data-ttu-id="def72-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="def72-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create projectParticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
