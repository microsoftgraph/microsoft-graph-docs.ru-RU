---
title: Создание Едукатионалактивити
description: Создание нового Едукатионалактивити.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9da437b7bc53d1d42c2d1f8fcc33d76925c8c8ef
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229348"
---
# <a name="create-educationalactivity"></a><span data-ttu-id="72ef1-103">Создание Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="72ef1-103">Create educationalActivity</span></span>

<span data-ttu-id="72ef1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72ef1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72ef1-105">Создайте новый [едукатионалактивити](../resources/educationalactivity.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="72ef1-105">Create a new [educationalActivity](../resources/educationalactivity.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="72ef1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72ef1-106">Permissions</span></span>

<span data-ttu-id="72ef1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72ef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72ef1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72ef1-109">Permission type</span></span>                        | <span data-ttu-id="72ef1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72ef1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72ef1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72ef1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72ef1-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="72ef1-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="72ef1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72ef1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72ef1-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="72ef1-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="72ef1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72ef1-115">Application</span></span>                            | <span data-ttu-id="72ef1-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72ef1-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="72ef1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72ef1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/educationalActivities
```

## <a name="request-headers"></a><span data-ttu-id="72ef1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72ef1-118">Request headers</span></span>

| <span data-ttu-id="72ef1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72ef1-119">Name</span></span>           |<span data-ttu-id="72ef1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="72ef1-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="72ef1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72ef1-121">Authorization</span></span>  | <span data-ttu-id="72ef1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72ef1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="72ef1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72ef1-124">Content-Type</span></span>   | <span data-ttu-id="72ef1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72ef1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72ef1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72ef1-127">Request body</span></span>

<span data-ttu-id="72ef1-128">В тексте запроса добавьте представление объекта [едукатионалактивити](../resources/educationalactivity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72ef1-128">In the request body, supply a JSON representation of an [educationalActivity](../resources/educationalactivity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="72ef1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="72ef1-129">Response</span></span>

<span data-ttu-id="72ef1-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [едукатионалактивити](../resources/educationalactivity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72ef1-130">If successful, this method returns a `201 Created` response code and a new [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72ef1-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="72ef1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72ef1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="72ef1-132">Request</span></span>

<span data-ttu-id="72ef1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72ef1-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72ef1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="72ef1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationalactivity_from_profile"
}-->

```http
POST /me/profile/educationalActivities
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
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
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```
# <a name="c"></a>[<span data-ttu-id="72ef1-135">C#</span><span class="sxs-lookup"><span data-stu-id="72ef1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationalactivity-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72ef1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72ef1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationalactivity-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72ef1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72ef1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationalactivity-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72ef1-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="72ef1-138">Response</span></span>

<span data-ttu-id="72ef1-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72ef1-139">The following is an example of the response.</span></span>

> <span data-ttu-id="72ef1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72ef1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
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
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
