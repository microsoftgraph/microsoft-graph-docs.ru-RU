---
title: Обновление Воркпоситион
description: Обновление свойств объекта Воркпоситион в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 48128b9c013456998fb8a7dcd7e502bbf7ad91b8
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996084"
---
# <a name="update-workposition"></a><span data-ttu-id="52f22-103">Обновление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="52f22-103">Update workPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52f22-104">Обновление свойств объекта [воркпоситион](../resources/workposition.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="52f22-104">Update the properties of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="52f22-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52f22-105">Permissions</span></span>

<span data-ttu-id="52f22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52f22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52f22-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52f22-108">Permission type</span></span>                        | <span data-ttu-id="52f22-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52f22-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52f22-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52f22-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="52f22-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="52f22-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="52f22-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52f22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52f22-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="52f22-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="52f22-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52f22-114">Application</span></span>                            | <span data-ttu-id="52f22-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52f22-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="52f22-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52f22-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="52f22-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52f22-117">Request headers</span></span>

| <span data-ttu-id="52f22-118">Имя</span><span class="sxs-lookup"><span data-stu-id="52f22-118">Name</span></span>           |<span data-ttu-id="52f22-119">Описание</span><span class="sxs-lookup"><span data-stu-id="52f22-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="52f22-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52f22-120">Authorization</span></span>  | <span data-ttu-id="52f22-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52f22-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="52f22-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52f22-123">Content-Type</span></span>   | <span data-ttu-id="52f22-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52f22-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="52f22-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52f22-126">Request body</span></span>

<span data-ttu-id="52f22-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="52f22-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="52f22-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="52f22-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="52f22-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="52f22-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="52f22-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="52f22-130">Property</span></span>     | <span data-ttu-id="52f22-131">Тип</span><span class="sxs-lookup"><span data-stu-id="52f22-131">Type</span></span>                                        | <span data-ttu-id="52f22-132">Описание</span><span class="sxs-lookup"><span data-stu-id="52f22-132">Description</span></span>                                                                                                 |
|:-------------|:--------------------------------------------|:------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="52f22-133">categories</span><span class="sxs-lookup"><span data-stu-id="52f22-133">categories</span></span>|<span data-ttu-id="52f22-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="52f22-134">String collection</span></span>                                | <span data-ttu-id="52f22-135">Содержит категории, связанные с положением пользователя.</span><span class="sxs-lookup"><span data-stu-id="52f22-135">Contains categories a user has associated with the position.</span></span> <span data-ttu-id="52f22-136">(например: цифровое преобразование, MS Graph, люди)</span><span class="sxs-lookup"><span data-stu-id="52f22-136">(eg: digital transformation, ms graph, people)</span></span> |
|<span data-ttu-id="52f22-137">описаны</span><span class="sxs-lookup"><span data-stu-id="52f22-137">detail</span></span>    |[<span data-ttu-id="52f22-138">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="52f22-138">positionDetail</span></span>](../resources/positiondetail.md) | <span data-ttu-id="52f22-139">Содержит подробные сведения о положении, в котором работают пользователи.</span><span class="sxs-lookup"><span data-stu-id="52f22-139">Contains detail about a users work position.</span></span>                                                                |

## <a name="response"></a><span data-ttu-id="52f22-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="52f22-140">Response</span></span>

<span data-ttu-id="52f22-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркпоситион](../resources/workposition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52f22-141">If successful, this method returns a `200 OK` response code and an updated [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52f22-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="52f22-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52f22-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="52f22-143">Request</span></span>

<span data-ttu-id="52f22-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52f22-144">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="52f22-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="52f22-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workposition"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/positions/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
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
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="52f22-146">C#</span><span class="sxs-lookup"><span data-stu-id="52f22-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52f22-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52f22-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52f22-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52f22-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="52f22-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="52f22-149">Response</span></span>

<span data-ttu-id="52f22-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="52f22-150">The following is an example of the response.</span></span>

> <span data-ttu-id="52f22-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52f22-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
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
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workposition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
