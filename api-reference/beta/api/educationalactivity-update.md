---
title: Обновление едукатионалактивити
description: Обновление свойств объекта Едукатионалактивити.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 886bfa6fc9271c633689b725584bd0c57d3fc4fc
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510634"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="0b9d1-103">Обновление едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="0b9d1-103">Update educationalactivity</span></span>

<span data-ttu-id="0b9d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b9d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b9d1-105">Обновление свойств объекта [едукатионалактивити](../resources/educationalactivity.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-105">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b9d1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b9d1-106">Permissions</span></span>

<span data-ttu-id="0b9d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b9d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b9d1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b9d1-109">Permission type</span></span>                        | <span data-ttu-id="0b9d1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b9d1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0b9d1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b9d1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b9d1-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0b9d1-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0b9d1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b9d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b9d1-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0b9d1-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0b9d1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b9d1-115">Application</span></span>                            | <span data-ttu-id="0b9d1-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b9d1-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0b9d1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b9d1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="0b9d1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b9d1-118">Request headers</span></span>

| <span data-ttu-id="0b9d1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0b9d1-119">Name</span></span>           |<span data-ttu-id="0b9d1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0b9d1-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0b9d1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b9d1-121">Authorization</span></span>  | <span data-ttu-id="0b9d1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0b9d1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b9d1-124">Content-Type</span></span>   | <span data-ttu-id="0b9d1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b9d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b9d1-127">Request body</span></span>

<span data-ttu-id="0b9d1-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0b9d1-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0b9d1-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0b9d1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b9d1-131">Property</span></span>           | <span data-ttu-id="0b9d1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0b9d1-132">Type</span></span>                                                                  | <span data-ttu-id="0b9d1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0b9d1-133">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="0b9d1-134">комплетионмонсеар</span><span class="sxs-lookup"><span data-stu-id="0b9d1-134">completionMonthYear</span></span> |<span data-ttu-id="0b9d1-135">Дата</span><span class="sxs-lookup"><span data-stu-id="0b9d1-135">Date</span></span>                                                                   | <span data-ttu-id="0b9d1-136">Месяц и год, когда пользователь выполнит или выполнил действие.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-136">The month and year the user graduated or completed the activity.</span></span>           |
|<span data-ttu-id="0b9d1-137">ендмонсеар</span><span class="sxs-lookup"><span data-stu-id="0b9d1-137">endMonthYear</span></span>        |<span data-ttu-id="0b9d1-138">Дата</span><span class="sxs-lookup"><span data-stu-id="0b9d1-138">Date</span></span>                                                                   | <span data-ttu-id="0b9d1-139">Месяц и год, когда пользователь завершил действие учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-139">The month and year the user completed the educational activity referenced.</span></span> |
|<span data-ttu-id="0b9d1-140">Организация</span><span class="sxs-lookup"><span data-stu-id="0b9d1-140">institution</span></span>         |[<span data-ttu-id="0b9d1-141">институтиондата</span><span class="sxs-lookup"><span data-stu-id="0b9d1-141">institutionData</span></span>](../resources/institutiondata.md)                     | <span data-ttu-id="0b9d1-142">Содержит подробные сведения о учебном заведения.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-142">Contains details of the institution studied at.</span></span>                            |
|<span data-ttu-id="0b9d1-143">Программа</span><span class="sxs-lookup"><span data-stu-id="0b9d1-143">program</span></span>             |[<span data-ttu-id="0b9d1-144">едукатионалактивитидетаил</span><span class="sxs-lookup"><span data-stu-id="0b9d1-144">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md) | <span data-ttu-id="0b9d1-145">Содержит расширенные сведения о программе или курсе.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-145">Contains extended information about the program or course.</span></span>                 |
|<span data-ttu-id="0b9d1-146">стартмонсеар</span><span class="sxs-lookup"><span data-stu-id="0b9d1-146">startMonthYear</span></span>      |<span data-ttu-id="0b9d1-147">Дата</span><span class="sxs-lookup"><span data-stu-id="0b9d1-147">Date</span></span>                                                                   | <span data-ttu-id="0b9d1-148">Месяц и год, когда пользователь присвоено указанному действию.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-148">The month and year the user commenced the activity referenced.</span></span>             |

## <a name="response"></a><span data-ttu-id="0b9d1-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b9d1-149">Response</span></span>

<span data-ttu-id="0b9d1-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [едукатионалактивити](../resources/educationalactivity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-150">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b9d1-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b9d1-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b9d1-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b9d1-152">Request</span></span>

<span data-ttu-id="0b9d1-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b9d1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b9d1-154">HTTP</span></span>](#tab/http)

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

# <a name="c"></a>[<span data-ttu-id="0b9d1-155">C#</span><span class="sxs-lookup"><span data-stu-id="0b9d1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b9d1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b9d1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b9d1-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b9d1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0b9d1-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b9d1-158">Response</span></span>

<span data-ttu-id="0b9d1-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-159">The following is an example of the response.</span></span>

> <span data-ttu-id="0b9d1-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b9d1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
