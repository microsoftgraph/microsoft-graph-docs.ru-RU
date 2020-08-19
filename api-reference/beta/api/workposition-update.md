---
title: Обновление Воркпоситион
description: Обновление свойств объекта Воркпоситион в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8c814f81a9ffbbb6f9e962c770a9a8908b288cde
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812830"
---
# <a name="update-workposition"></a><span data-ttu-id="e383d-103">Обновление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="e383d-103">Update workPosition</span></span>

<span data-ttu-id="e383d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e383d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e383d-105">Обновление свойств объекта [воркпоситион](../resources/workposition.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="e383d-105">Update the properties of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e383d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e383d-106">Permissions</span></span>

<span data-ttu-id="e383d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e383d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e383d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e383d-109">Permission type</span></span>                        | <span data-ttu-id="e383d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e383d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e383d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e383d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e383d-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e383d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e383d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e383d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e383d-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e383d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e383d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e383d-115">Application</span></span>                            | <span data-ttu-id="e383d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e383d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e383d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e383d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/positions/{id}
PATCH /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e383d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e383d-118">Request headers</span></span>

| <span data-ttu-id="e383d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e383d-119">Name</span></span>           |<span data-ttu-id="e383d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e383d-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e383d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e383d-121">Authorization</span></span>  | <span data-ttu-id="e383d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e383d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e383d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e383d-124">Content-Type</span></span>   | <span data-ttu-id="e383d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e383d-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e383d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e383d-127">Request body</span></span>

<span data-ttu-id="e383d-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e383d-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e383d-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e383d-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e383d-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e383d-130">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="properties"></a><span data-ttu-id="e383d-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="e383d-131">Properties</span></span>
|<span data-ttu-id="e383d-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="e383d-132">Property</span></span>|<span data-ttu-id="e383d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="e383d-133">Type</span></span>|<span data-ttu-id="e383d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e383d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e383d-135">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="e383d-135">allowedAudiences</span></span>|<span data-ttu-id="e383d-136">String</span><span class="sxs-lookup"><span data-stu-id="e383d-136">String</span></span>|<span data-ttu-id="e383d-137">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="e383d-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e383d-138">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e383d-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e383d-139">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e383d-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e383d-140">categories</span><span class="sxs-lookup"><span data-stu-id="e383d-140">categories</span></span>|<span data-ttu-id="e383d-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e383d-141">String collection</span></span>|<span data-ttu-id="e383d-142">Категории, связанные с этим положением пользователя.</span><span class="sxs-lookup"><span data-stu-id="e383d-142">Categories that the user has associated with this position.</span></span>|
|<span data-ttu-id="e383d-143">коллег</span><span class="sxs-lookup"><span data-stu-id="e383d-143">colleagues</span></span>|<span data-ttu-id="e383d-144">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="e383d-144">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="e383d-145">Коллеги, связанные с этой позицией.</span><span class="sxs-lookup"><span data-stu-id="e383d-145">Colleagues that are associated with this position.</span></span>|
|<span data-ttu-id="e383d-146">описаны</span><span class="sxs-lookup"><span data-stu-id="e383d-146">detail</span></span>|[<span data-ttu-id="e383d-147">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="e383d-147">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="e383d-148">Содержит подробные сведения о позиции.</span><span class="sxs-lookup"><span data-stu-id="e383d-148">Contains detailed information about the position.</span></span> |
|<span data-ttu-id="e383d-149">выводов</span><span class="sxs-lookup"><span data-stu-id="e383d-149">inference</span></span>|[<span data-ttu-id="e383d-150">инференцедата</span><span class="sxs-lookup"><span data-stu-id="e383d-150">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e383d-151">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="e383d-151">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e383d-152">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e383d-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e383d-153">по току</span><span class="sxs-lookup"><span data-stu-id="e383d-153">isCurrent</span></span>|<span data-ttu-id="e383d-154">Логический</span><span class="sxs-lookup"><span data-stu-id="e383d-154">Boolean</span></span>|<span data-ttu-id="e383d-155">Указывает, является ли должность текущей.</span><span class="sxs-lookup"><span data-stu-id="e383d-155">Denotes whether or not the position is current.</span></span>|
|<span data-ttu-id="e383d-156">manager</span><span class="sxs-lookup"><span data-stu-id="e383d-156">manager</span></span>|[<span data-ttu-id="e383d-157">релатедперсон</span><span class="sxs-lookup"><span data-stu-id="e383d-157">relatedPerson</span></span>](../resources/relatedperson.md)|<span data-ttu-id="e383d-158">Содержит сведения о руководителе пользователя в этой позиции.</span><span class="sxs-lookup"><span data-stu-id="e383d-158">Contains detail of the user's manager in this position.</span></span>|

## <a name="response"></a><span data-ttu-id="e383d-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="e383d-159">Response</span></span>

<span data-ttu-id="e383d-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркпоситион](../resources/workposition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e383d-160">If successful, this method returns a `200 OK` response code and an updated [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e383d-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="e383d-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e383d-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="e383d-162">Request</span></span>

<span data-ttu-id="e383d-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e383d-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e383d-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="e383d-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workposition"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/positions/{id}
Content-type: application/json

{
  "isCurrent": true
}
```
# <a name="c"></a>[<span data-ttu-id="e383d-165">C#</span><span class="sxs-lookup"><span data-stu-id="e383d-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e383d-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e383d-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e383d-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e383d-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e383d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="e383d-168">Response</span></span>

<span data-ttu-id="e383d-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e383d-169">The following is an example of the response.</span></span>

> <span data-ttu-id="e383d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e383d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
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
  "categories": null,
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "postOfficeBox": null,
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "state": null,
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "description": null,
    "endMonthYear": null,
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting",
    "startMonthYear": "datetime-value",
    "summary": null
  },
  "manager": null,
  "colleagues": null,
  "isCurrent": true
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
