---
title: Обновление едукатионалактивити
description: Обновление свойств объекта едукатионалактивити.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 68d9c6d2499b3610361ab0fdc2b78c188853b65b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994769"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="3805a-103">Обновление едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="3805a-103">Update educationalactivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3805a-104">Обновление свойств объекта [едукатионалактивити](../resources/educationalactivity.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="3805a-104">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3805a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3805a-105">Permissions</span></span>

<span data-ttu-id="3805a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3805a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3805a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3805a-108">Permission type</span></span>                        | <span data-ttu-id="3805a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3805a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3805a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3805a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3805a-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3805a-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3805a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3805a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3805a-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3805a-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3805a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3805a-114">Application</span></span>                            | <span data-ttu-id="3805a-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3805a-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3805a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3805a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="3805a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3805a-117">Request headers</span></span>

| <span data-ttu-id="3805a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3805a-118">Name</span></span>           |<span data-ttu-id="3805a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3805a-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="3805a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3805a-120">Authorization</span></span>  | <span data-ttu-id="3805a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3805a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3805a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3805a-123">Content-Type</span></span>   | <span data-ttu-id="3805a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3805a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3805a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3805a-126">Request body</span></span>

<span data-ttu-id="3805a-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3805a-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3805a-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="3805a-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3805a-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3805a-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3805a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3805a-130">Property</span></span>           | <span data-ttu-id="3805a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3805a-131">Type</span></span>                                                                  | <span data-ttu-id="3805a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3805a-132">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="3805a-133">комплетионмонсеар</span><span class="sxs-lookup"><span data-stu-id="3805a-133">completionMonthYear</span></span> |<span data-ttu-id="3805a-134">Дата</span><span class="sxs-lookup"><span data-stu-id="3805a-134">Date</span></span>                                                                   | <span data-ttu-id="3805a-135">Месяц и год, когда пользователь выполнит или выполнил действие.</span><span class="sxs-lookup"><span data-stu-id="3805a-135">The month and year the user graduated or completed the activity.</span></span>           |
|<span data-ttu-id="3805a-136">ендмонсеар</span><span class="sxs-lookup"><span data-stu-id="3805a-136">endMonthYear</span></span>        |<span data-ttu-id="3805a-137">Дата</span><span class="sxs-lookup"><span data-stu-id="3805a-137">Date</span></span>                                                                   | <span data-ttu-id="3805a-138">Месяц и год, когда пользователь завершил действие учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="3805a-138">The month and year the user completed the educational activity referenced.</span></span> |
|<span data-ttu-id="3805a-139">Организация</span><span class="sxs-lookup"><span data-stu-id="3805a-139">institution</span></span>         |[<span data-ttu-id="3805a-140">институтиондата</span><span class="sxs-lookup"><span data-stu-id="3805a-140">institutionData</span></span>](../resources/institutiondata.md)                     | <span data-ttu-id="3805a-141">Содержит подробные сведения о учебном заведения.</span><span class="sxs-lookup"><span data-stu-id="3805a-141">Contains details of the institution studied at.</span></span>                            |
|<span data-ttu-id="3805a-142">Программа</span><span class="sxs-lookup"><span data-stu-id="3805a-142">program</span></span>             |[<span data-ttu-id="3805a-143">едукатионалактивитидетаил</span><span class="sxs-lookup"><span data-stu-id="3805a-143">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md) | <span data-ttu-id="3805a-144">Содержит расширенные сведения о программе или курсе.</span><span class="sxs-lookup"><span data-stu-id="3805a-144">Contains extended information about the program or course.</span></span>                 |
|<span data-ttu-id="3805a-145">стартмонсеар</span><span class="sxs-lookup"><span data-stu-id="3805a-145">startMonthYear</span></span>      |<span data-ttu-id="3805a-146">Дата</span><span class="sxs-lookup"><span data-stu-id="3805a-146">Date</span></span>                                                                   | <span data-ttu-id="3805a-147">Месяц и год, когда пользователь присвоено указанному действию.</span><span class="sxs-lookup"><span data-stu-id="3805a-147">The month and year the user commenced the activity referenced.</span></span>             |

## <a name="response"></a><span data-ttu-id="3805a-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="3805a-148">Response</span></span>

<span data-ttu-id="3805a-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [едукатионалактивити](../resources/educationalactivity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3805a-149">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3805a-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="3805a-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3805a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="3805a-151">Request</span></span>

<span data-ttu-id="3805a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3805a-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3805a-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="3805a-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationalactivity"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3805a-154">C#</span><span class="sxs-lookup"><span data-stu-id="3805a-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3805a-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3805a-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3805a-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3805a-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3805a-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3805a-157">Response</span></span>

<span data-ttu-id="3805a-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3805a-158">The following is an example of the response.</span></span>

> <span data-ttu-id="3805a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3805a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Update educationalactivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
