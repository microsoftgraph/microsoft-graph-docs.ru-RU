---
title: Обновление образовательной активности
description: Обновление свойств объекта educationalActivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7f59b6ef2b5bebb2369a3cbd44baaae6ca209b97
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044489"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="f4f48-103">Обновление образовательной активности</span><span class="sxs-lookup"><span data-stu-id="f4f48-103">Update educationalactivity</span></span>

<span data-ttu-id="f4f48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4f48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4f48-105">Обновление свойств объекта [educationalActivity](../resources/educationalactivity.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="f4f48-105">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4f48-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4f48-106">Permissions</span></span>

<span data-ttu-id="f4f48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4f48-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4f48-109">Permission type</span></span>                        | <span data-ttu-id="f4f48-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4f48-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f4f48-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4f48-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4f48-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f48-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f4f48-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4f48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4f48-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f48-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f4f48-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4f48-115">Application</span></span>                            | <span data-ttu-id="f4f48-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f48-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f4f48-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4f48-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id}
PATCH /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f4f48-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4f48-118">Request headers</span></span>

| <span data-ttu-id="f4f48-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f4f48-119">Name</span></span>           |<span data-ttu-id="f4f48-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f4f48-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f4f48-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4f48-121">Authorization</span></span>  | <span data-ttu-id="f4f48-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4f48-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f4f48-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4f48-124">Content-Type</span></span>   | <span data-ttu-id="f4f48-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4f48-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4f48-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4f48-127">Request body</span></span>

<span data-ttu-id="f4f48-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f4f48-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f4f48-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f4f48-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f4f48-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f4f48-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="f4f48-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4f48-131">Property</span></span>|<span data-ttu-id="f4f48-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f4f48-132">Type</span></span>|<span data-ttu-id="f4f48-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f4f48-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f48-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="f4f48-134">allowedAudiences</span></span>|<span data-ttu-id="f4f48-135">String</span><span class="sxs-lookup"><span data-stu-id="f4f48-135">String</span></span>|<span data-ttu-id="f4f48-136">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="f4f48-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="f4f48-137">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f4f48-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="f4f48-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f4f48-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f4f48-139">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="f4f48-139">completionMonthYear</span></span>|<span data-ttu-id="f4f48-140">Date</span><span class="sxs-lookup"><span data-stu-id="f4f48-140">Date</span></span>|<span data-ttu-id="f4f48-141">Месяц и год, когда пользователь закончил или завершил действие.</span><span class="sxs-lookup"><span data-stu-id="f4f48-141">The month and year the user graduated or completed the activity.</span></span> |
|<span data-ttu-id="f4f48-142">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="f4f48-142">endMonthYear</span></span>|<span data-ttu-id="f4f48-143">Date</span><span class="sxs-lookup"><span data-stu-id="f4f48-143">Date</span></span>|<span data-ttu-id="f4f48-144">Месяц и год, когда пользователь завершил ссылаемую образовательную деятельность.</span><span class="sxs-lookup"><span data-stu-id="f4f48-144">The month and year the user completed the educational activity referenced.</span></span>|
|<span data-ttu-id="f4f48-145">вывод</span><span class="sxs-lookup"><span data-stu-id="f4f48-145">inference</span></span>|[<span data-ttu-id="f4f48-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="f4f48-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="f4f48-147">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="f4f48-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="f4f48-148">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f4f48-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f4f48-149">учреждение</span><span class="sxs-lookup"><span data-stu-id="f4f48-149">institution</span></span>|[<span data-ttu-id="f4f48-150">institutionData</span><span class="sxs-lookup"><span data-stu-id="f4f48-150">institutionData</span></span>](../resources/institutiondata.md)|<span data-ttu-id="f4f48-151">Содержит сведения об изучаемом учреждении.</span><span class="sxs-lookup"><span data-stu-id="f4f48-151">Contains details of the institution studied at.</span></span> |
|<span data-ttu-id="f4f48-152">программа</span><span class="sxs-lookup"><span data-stu-id="f4f48-152">program</span></span>|[<span data-ttu-id="f4f48-153">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="f4f48-153">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md)|<span data-ttu-id="f4f48-154">Содержит расширенные сведения о программе или курсе.</span><span class="sxs-lookup"><span data-stu-id="f4f48-154">Contains extended information about the program or course.</span></span>|
|<span data-ttu-id="f4f48-155">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="f4f48-155">startMonthYear</span></span>|<span data-ttu-id="f4f48-156">Date</span><span class="sxs-lookup"><span data-stu-id="f4f48-156">Date</span></span>|<span data-ttu-id="f4f48-157">Месяц и год, когда пользователь начал со ссылкой на действие.</span><span class="sxs-lookup"><span data-stu-id="f4f48-157">The month and year the user commenced the activity referenced.</span></span>|

## <a name="response"></a><span data-ttu-id="f4f48-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4f48-158">Response</span></span>

<span data-ttu-id="f4f48-159">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект educationalActivity](../resources/educationalactivity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f4f48-159">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4f48-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="f4f48-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4f48-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4f48-161">Request</span></span>

<span data-ttu-id="f4f48-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4f48-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4f48-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4f48-163">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationalactivity"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
Content-type: application/json

{
  "institution": {
    "location": {
      "type": "business",
      "postOfficeBox": null,
      "street": "12000 E Prospect Rd",
      "city": "Fort Collins",
      "state": "Colorado",
      "countryOrRegion": "USA",
      "postalCode": "80525"
    }
  }
}
```

# <a name="c"></a>[<span data-ttu-id="f4f48-164">C#</span><span class="sxs-lookup"><span data-stu-id="f4f48-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4f48-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4f48-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4f48-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4f48-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4f48-167">Java</span><span class="sxs-lookup"><span data-stu-id="f4f48-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationalactivity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f4f48-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4f48-168">Response</span></span>

<span data-ttu-id="f4f48-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f4f48-169">The following is an example of the response.</span></span>

> <span data-ttu-id="f4f48-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f4f48-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "description": null,
    "displayName": "Colorado State University",
    "location": {
      "type": "business",
      "postOfficeBox": null,
      "street": "12000 E Prospect Rd",
      "city": "Fort Collins",
      "state": "Colorado",
      "countryOrRegion": "USA",
      "postalCode": "80525"
    },
    "webUrl": "https://www.colostate.edu"
  },
  "program": {
    "abbreviation": "MBA",
    "activities": null,
    "awards": null,
    "description": "Master of Business Administration with a major in Entreprenuership and Finance.",
    "displayName": "Master of Business Administration",
    "fieldsOfStudy": null,
    "grade": "3.9",
    "notes": null,
    "webUrl": "https://biz.colostate.edu"
  },
  "startMonthYear": "Date"
}
```


