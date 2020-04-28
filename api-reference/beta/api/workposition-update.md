---
title: Обновление Воркпоситион
description: Обновление свойств объекта Воркпоситион в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 04a3dc0a0580db1f41daa1e08ba8c7e196e02dcb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451314"
---
# <a name="update-workposition"></a><span data-ttu-id="08a41-103">Обновление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="08a41-103">Update workPosition</span></span>

<span data-ttu-id="08a41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08a41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08a41-105">Обновление свойств объекта [воркпоситион](../resources/workposition.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="08a41-105">Update the properties of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="08a41-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08a41-106">Permissions</span></span>

<span data-ttu-id="08a41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08a41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08a41-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08a41-109">Permission type</span></span>                        | <span data-ttu-id="08a41-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08a41-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="08a41-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08a41-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08a41-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="08a41-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="08a41-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08a41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08a41-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="08a41-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="08a41-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08a41-115">Application</span></span>                            | <span data-ttu-id="08a41-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a41-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="08a41-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08a41-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="08a41-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08a41-118">Request headers</span></span>

| <span data-ttu-id="08a41-119">Имя</span><span class="sxs-lookup"><span data-stu-id="08a41-119">Name</span></span>           |<span data-ttu-id="08a41-120">Описание</span><span class="sxs-lookup"><span data-stu-id="08a41-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="08a41-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08a41-121">Authorization</span></span>  | <span data-ttu-id="08a41-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08a41-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="08a41-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08a41-124">Content-Type</span></span>   | <span data-ttu-id="08a41-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08a41-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="08a41-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08a41-127">Request body</span></span>

<span data-ttu-id="08a41-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="08a41-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="08a41-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="08a41-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="08a41-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="08a41-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="08a41-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="08a41-131">Property</span></span>     | <span data-ttu-id="08a41-132">Тип</span><span class="sxs-lookup"><span data-stu-id="08a41-132">Type</span></span>                                        | <span data-ttu-id="08a41-133">Описание</span><span class="sxs-lookup"><span data-stu-id="08a41-133">Description</span></span>                                                                                                 |
|:-------------|:--------------------------------------------|:------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="08a41-134">categories</span><span class="sxs-lookup"><span data-stu-id="08a41-134">categories</span></span>|<span data-ttu-id="08a41-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="08a41-135">String collection</span></span>                                | <span data-ttu-id="08a41-136">Содержит категории, связанные с положением пользователя.</span><span class="sxs-lookup"><span data-stu-id="08a41-136">Contains categories a user has associated with the position.</span></span> <span data-ttu-id="08a41-137">(например: цифровое преобразование, MS Graph, люди)</span><span class="sxs-lookup"><span data-stu-id="08a41-137">(eg: digital transformation, ms graph, people)</span></span> |
|<span data-ttu-id="08a41-138">описаны</span><span class="sxs-lookup"><span data-stu-id="08a41-138">detail</span></span>    |[<span data-ttu-id="08a41-139">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="08a41-139">positionDetail</span></span>](../resources/positiondetail.md) | <span data-ttu-id="08a41-140">Содержит подробные сведения о положении, в котором работают пользователи.</span><span class="sxs-lookup"><span data-stu-id="08a41-140">Contains detail about a users work position.</span></span>                                                                |

## <a name="response"></a><span data-ttu-id="08a41-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="08a41-141">Response</span></span>

<span data-ttu-id="08a41-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркпоситион](../resources/workposition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08a41-142">If successful, this method returns a `200 OK` response code and an updated [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08a41-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="08a41-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08a41-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="08a41-144">Request</span></span>

<span data-ttu-id="08a41-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08a41-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08a41-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="08a41-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="08a41-147">C#</span><span class="sxs-lookup"><span data-stu-id="08a41-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08a41-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08a41-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08a41-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08a41-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08a41-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="08a41-150">Response</span></span>

<span data-ttu-id="08a41-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08a41-151">The following is an example of the response.</span></span>

> <span data-ttu-id="08a41-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08a41-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
