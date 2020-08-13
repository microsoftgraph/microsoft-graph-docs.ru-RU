---
title: Обновление типа ресурса ПрожектпартиЦипатион
description: Обновление свойств объекта ПрожектпартиЦипатион в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b0aa9353a9e16929bd71f41f5328c0fdaf12c531
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454929"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="d2175-103">Обновление прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="d2175-103">Update projectparticipation</span></span>

<span data-ttu-id="d2175-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2175-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2175-105">Обновление свойств объекта [прожектпартиЦипатион](../resources/projectParticipation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2175-105">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2175-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2175-106">Permissions</span></span>

<span data-ttu-id="d2175-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2175-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2175-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2175-109">Permission type</span></span>                        | <span data-ttu-id="d2175-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2175-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2175-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2175-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2175-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d2175-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d2175-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2175-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2175-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d2175-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d2175-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2175-115">Application</span></span>                            | <span data-ttu-id="d2175-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2175-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d2175-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2175-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d2175-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2175-118">Request headers</span></span>

| <span data-ttu-id="d2175-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d2175-119">Name</span></span>           |<span data-ttu-id="d2175-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d2175-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d2175-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2175-121">Authorization</span></span>  | <span data-ttu-id="d2175-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2175-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d2175-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2175-124">Content-Type</span></span>   | <span data-ttu-id="d2175-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2175-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d2175-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2175-127">Request body</span></span>

<span data-ttu-id="d2175-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d2175-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d2175-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d2175-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d2175-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d2175-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d2175-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2175-131">Property</span></span>     | <span data-ttu-id="d2175-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d2175-132">Type</span></span>                                                     | <span data-ttu-id="d2175-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d2175-133">Description</span></span>                                                                                        |
|:-------------|:---------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d2175-134">categories</span><span class="sxs-lookup"><span data-stu-id="d2175-134">categories</span></span>    |<span data-ttu-id="d2175-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d2175-135">String collection</span></span>                                         | <span data-ttu-id="d2175-136">Содержит категории, связанные с проектом пользователем (например, цифровое преобразование, на платформе для нефтегазовой платформы)</span><span class="sxs-lookup"><span data-stu-id="d2175-136">Contains categories a user has associated with the project (eg: digital transformation, oil rig)</span></span>   |
|<span data-ttu-id="d2175-137">Клиенты</span><span class="sxs-lookup"><span data-stu-id="d2175-137">client</span></span>        |[<span data-ttu-id="d2175-138">компанидетаил</span><span class="sxs-lookup"><span data-stu-id="d2175-138">companyDetail</span></span>](../resources/companydetail.md)            | <span data-ttu-id="d2175-139">Содержит подробные сведения о клиенте, для которого выполнялся проект.</span><span class="sxs-lookup"><span data-stu-id="d2175-139">Contains detailed information about the client the project was for.</span></span>                                |
|<span data-ttu-id="d2175-140">коллег</span><span class="sxs-lookup"><span data-stu-id="d2175-140">colleagues</span></span>    |<span data-ttu-id="d2175-141">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="d2175-141">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="d2175-142">Пользователи, которые также работали над проектом.</span><span class="sxs-lookup"><span data-stu-id="d2175-142">People that also worked on the project.</span></span>                                                            |
|<span data-ttu-id="d2175-143">описаны</span><span class="sxs-lookup"><span data-stu-id="d2175-143">detail</span></span>        |[<span data-ttu-id="d2175-144">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="d2175-144">positionDetail</span></span>](../resources/positiondetail.md)          | <span data-ttu-id="d2175-145">Содержит подробные сведения о роли пользователей в проекте.</span><span class="sxs-lookup"><span data-stu-id="d2175-145">Contains detail about the users role on the project.</span></span>                                               |
|<span data-ttu-id="d2175-146">displayName</span><span class="sxs-lookup"><span data-stu-id="d2175-146">displayName</span></span>   |<span data-ttu-id="d2175-147">Строка</span><span class="sxs-lookup"><span data-stu-id="d2175-147">String</span></span>                                                    | <span data-ttu-id="d2175-148">Содержит понятное имя проекта.</span><span class="sxs-lookup"><span data-stu-id="d2175-148">Contains a friendly name for the project.</span></span>                                                          |
|<span data-ttu-id="d2175-149">спонсорами</span><span class="sxs-lookup"><span data-stu-id="d2175-149">sponsors</span></span>      |<span data-ttu-id="d2175-150">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="d2175-150">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="d2175-151">Пользователь (люди), который спонсор проекта.</span><span class="sxs-lookup"><span data-stu-id="d2175-151">Person(People) who sponsored the project.</span></span>                                                          |

## <a name="response"></a><span data-ttu-id="d2175-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2175-152">Response</span></span>

<span data-ttu-id="d2175-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [прожектпартиЦипатион](../resources/projectparticipation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2175-153">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2175-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2175-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2175-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2175-155">Request</span></span>

<span data-ttu-id="d2175-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2175-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2175-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2175-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_projectparticipation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/projects/{id}
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
# <a name="c"></a>[<span data-ttu-id="d2175-158">C#</span><span class="sxs-lookup"><span data-stu-id="d2175-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2175-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2175-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2175-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2175-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2175-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2175-161">Response</span></span>

<span data-ttu-id="d2175-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2175-162">The following is an example of the response.</span></span>

> <span data-ttu-id="d2175-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2175-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Update projectparticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
