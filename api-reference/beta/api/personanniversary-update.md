---
title: Обновление personAnniversary
description: Обновление свойств объекта personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7506a62e45246de610ab31d6cd04fa042b0492c4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037853"
---
# <a name="update-personanniversary"></a><span data-ttu-id="dd32b-103">Обновление personAnniversary</span><span class="sxs-lookup"><span data-stu-id="dd32b-103">Update personAnniversary</span></span>

<span data-ttu-id="dd32b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd32b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd32b-105">Обновление свойств объекта [personAnniversary](../resources/personanniversary.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="dd32b-105">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd32b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd32b-106">Permissions</span></span>

<span data-ttu-id="dd32b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd32b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd32b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd32b-109">Permission type</span></span>                        | <span data-ttu-id="dd32b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd32b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd32b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd32b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd32b-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd32b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="dd32b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd32b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd32b-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd32b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="dd32b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd32b-115">Application</span></span>                            | <span data-ttu-id="dd32b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd32b-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="dd32b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd32b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id}
PATCH /users/{id | userPrincipalName}/profile/anniversaries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dd32b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd32b-118">Request headers</span></span>

| <span data-ttu-id="dd32b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dd32b-119">Name</span></span>           |<span data-ttu-id="dd32b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dd32b-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="dd32b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd32b-121">Authorization</span></span>  | <span data-ttu-id="dd32b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd32b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="dd32b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd32b-124">Content-Type</span></span>   | <span data-ttu-id="dd32b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd32b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd32b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd32b-127">Request body</span></span>

<span data-ttu-id="dd32b-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="dd32b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dd32b-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="dd32b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dd32b-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dd32b-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="dd32b-131">В следующей таблице показаны свойства, которые можно обновить в существующем объекте [personAnniversary](../resources/personanniversary.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="dd32b-131">The following table shows the properties that are possible to update within an existing [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="dd32b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd32b-132">Property</span></span>|<span data-ttu-id="dd32b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="dd32b-133">Type</span></span>|<span data-ttu-id="dd32b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="dd32b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd32b-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="dd32b-135">allowedAudiences</span></span>|<span data-ttu-id="dd32b-136">String</span><span class="sxs-lookup"><span data-stu-id="dd32b-136">String</span></span>|<span data-ttu-id="dd32b-137">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="dd32b-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="dd32b-138">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="dd32b-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="dd32b-139">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dd32b-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dd32b-140">date</span><span class="sxs-lookup"><span data-stu-id="dd32b-140">date</span></span>|<span data-ttu-id="dd32b-141">Date</span><span class="sxs-lookup"><span data-stu-id="dd32b-141">Date</span></span>|<span data-ttu-id="dd32b-142">Содержит дату, связанную с юбилейным типом.</span><span class="sxs-lookup"><span data-stu-id="dd32b-142">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="dd32b-143">вывод</span><span class="sxs-lookup"><span data-stu-id="dd32b-143">inference</span></span>|[<span data-ttu-id="dd32b-144">inferenceData</span><span class="sxs-lookup"><span data-stu-id="dd32b-144">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="dd32b-145">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="dd32b-145">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="dd32b-146">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="dd32b-146">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="dd32b-147">type</span><span class="sxs-lookup"><span data-stu-id="dd32b-147">type</span></span>|<span data-ttu-id="dd32b-148">anniversaryType</span><span class="sxs-lookup"><span data-stu-id="dd32b-148">anniversaryType</span></span>|<span data-ttu-id="dd32b-149">Тип юбилея, который представляет дата.</span><span class="sxs-lookup"><span data-stu-id="dd32b-149">The type of anniversary the date represents.</span></span> <span data-ttu-id="dd32b-150">Возможные значения: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dd32b-150">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="dd32b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd32b-151">Response</span></span>

<span data-ttu-id="dd32b-152">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект personAnniversary](../resources/personanniversary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd32b-152">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd32b-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd32b-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd32b-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd32b-154">Request</span></span>

<span data-ttu-id="dd32b-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd32b-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd32b-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd32b-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personanniversary"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
Content-type: application/json

{
  "allowedAudiences": "contacts"
}
```
# <a name="c"></a>[<span data-ttu-id="dd32b-157">C#</span><span class="sxs-lookup"><span data-stu-id="dd32b-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd32b-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd32b-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd32b-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd32b-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd32b-160">Java</span><span class="sxs-lookup"><span data-stu-id="dd32b-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personanniversary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="dd32b-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd32b-161">Response</span></span>

<span data-ttu-id="dd32b-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dd32b-162">The following is an example of the response.</span></span>

> <span data-ttu-id="dd32b-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dd32b-163">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "contacts",
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
```


