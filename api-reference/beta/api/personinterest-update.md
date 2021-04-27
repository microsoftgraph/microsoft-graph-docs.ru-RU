---
title: Обновление personInterest
description: Обновление свойств объекта personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 50366a62d9f407ada0208169de202d106b1144eb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037818"
---
# <a name="update-personinterest"></a><span data-ttu-id="a817c-103">Обновление personinterest</span><span class="sxs-lookup"><span data-stu-id="a817c-103">Update personinterest</span></span>

<span data-ttu-id="a817c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a817c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a817c-105">Обновление свойств объекта [personInterest](../resources/personinterest.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="a817c-105">Update the properties of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a817c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a817c-106">Permissions</span></span>

<span data-ttu-id="a817c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a817c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a817c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a817c-109">Permission type</span></span>                        | <span data-ttu-id="a817c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a817c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a817c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a817c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a817c-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a817c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a817c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a817c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a817c-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a817c-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a817c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a817c-115">Application</span></span>                            | <span data-ttu-id="a817c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a817c-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="a817c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a817c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/interests/{id}
PATCH /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a817c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a817c-118">Request headers</span></span>

| <span data-ttu-id="a817c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a817c-119">Name</span></span>           |<span data-ttu-id="a817c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a817c-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a817c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a817c-121">Authorization</span></span>  | <span data-ttu-id="a817c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a817c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a817c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a817c-124">Content-Type</span></span>   | <span data-ttu-id="a817c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a817c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a817c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a817c-127">Request body</span></span>

<span data-ttu-id="a817c-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a817c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a817c-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a817c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a817c-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a817c-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="a817c-131">В следующей таблице показаны свойства, которые можно обновить в существующем [объекте personInterest](../resources/personinterest.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="a817c-131">The following table shows the properties that are possible to update within an existing [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="a817c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="a817c-132">Property</span></span>|<span data-ttu-id="a817c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a817c-133">Type</span></span>|<span data-ttu-id="a817c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a817c-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a817c-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="a817c-135">allowedAudiences</span></span>|<span data-ttu-id="a817c-136">String</span><span class="sxs-lookup"><span data-stu-id="a817c-136">String</span></span>|<span data-ttu-id="a817c-137">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="a817c-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="a817c-138">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a817c-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="a817c-139">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a817c-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a817c-140">categories</span><span class="sxs-lookup"><span data-stu-id="a817c-140">categories</span></span>|<span data-ttu-id="a817c-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a817c-141">String collection</span></span>|<span data-ttu-id="a817c-142">Содержит категории, связанные с интересом пользователя (например, личные, личные).</span><span class="sxs-lookup"><span data-stu-id="a817c-142">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="a817c-143">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="a817c-143">collaborationTags</span></span>|<span data-ttu-id="a817c-144">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a817c-144">String collection</span></span>|<span data-ttu-id="a817c-145">Содержит теги сценариев работы, которые пользователь связал с интересом.</span><span class="sxs-lookup"><span data-stu-id="a817c-145">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="a817c-146">Допустимые значения в коллекции: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="a817c-146">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="a817c-147">description</span><span class="sxs-lookup"><span data-stu-id="a817c-147">description</span></span>|<span data-ttu-id="a817c-148">String</span><span class="sxs-lookup"><span data-stu-id="a817c-148">String</span></span>|<span data-ttu-id="a817c-149">Содержит описание интерес.</span><span class="sxs-lookup"><span data-stu-id="a817c-149">Contains a description of the interest.</span></span>|
|<span data-ttu-id="a817c-150">displayName</span><span class="sxs-lookup"><span data-stu-id="a817c-150">displayName</span></span>|<span data-ttu-id="a817c-151">String</span><span class="sxs-lookup"><span data-stu-id="a817c-151">String</span></span>|<span data-ttu-id="a817c-152">Содержит удобное имя для интереса.</span><span class="sxs-lookup"><span data-stu-id="a817c-152">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="a817c-153">вывод</span><span class="sxs-lookup"><span data-stu-id="a817c-153">inference</span></span>|[<span data-ttu-id="a817c-154">inferenceData</span><span class="sxs-lookup"><span data-stu-id="a817c-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="a817c-155">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="a817c-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="a817c-156">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a817c-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a817c-157">webUrl</span><span class="sxs-lookup"><span data-stu-id="a817c-157">webUrl</span></span>|<span data-ttu-id="a817c-158">String</span><span class="sxs-lookup"><span data-stu-id="a817c-158">String</span></span>|<span data-ttu-id="a817c-159">Содержит ссылку на веб-страницу или ресурс об интересе.</span><span class="sxs-lookup"><span data-stu-id="a817c-159">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="a817c-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="a817c-160">Response</span></span>

<span data-ttu-id="a817c-161">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [personInterest](../resources/personinterest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a817c-161">If successful, this method returns a `200 OK` response code and an updated [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a817c-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="a817c-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a817c-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="a817c-163">Request</span></span>

<span data-ttu-id="a817c-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a817c-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a817c-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="a817c-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personinterest"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/interests/{id}
Content-type: application/json

{
  "categories": [
    "Sports"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a817c-166">C#</span><span class="sxs-lookup"><span data-stu-id="a817c-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a817c-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a817c-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a817c-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a817c-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a817c-169">Java</span><span class="sxs-lookup"><span data-stu-id="a817c-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personinterest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a817c-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="a817c-170">Response</span></span>

<span data-ttu-id="a817c-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a817c-171">The following is an example of the response.</span></span>

> <span data-ttu-id="a817c-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a817c-172">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
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
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


