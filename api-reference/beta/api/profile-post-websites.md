---
title: Создание personWebsite
description: Создание нового personWebsite.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f05a1cab47ef5500242cbda9fd0452a4e78a4750
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036712"
---
# <a name="create-personwebsite"></a><span data-ttu-id="e785d-103">Создание personWebsite</span><span class="sxs-lookup"><span data-stu-id="e785d-103">Create personWebsite</span></span>

<span data-ttu-id="e785d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e785d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e785d-105">Создание нового [объекта personWebsite](../resources/personwebsite.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="e785d-105">Create a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e785d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e785d-106">Permissions</span></span>

<span data-ttu-id="e785d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e785d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e785d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e785d-109">Permission type</span></span>                        | <span data-ttu-id="e785d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e785d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e785d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e785d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e785d-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e785d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e785d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e785d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e785d-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e785d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e785d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e785d-115">Application</span></span>                            | <span data-ttu-id="e785d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e785d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e785d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e785d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/websites
POST /users/{id | userPrincipalName}/profile/websites
```

## <a name="request-headers"></a><span data-ttu-id="e785d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e785d-118">Request headers</span></span>

| <span data-ttu-id="e785d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e785d-119">Name</span></span>           | <span data-ttu-id="e785d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e785d-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="e785d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e785d-121">Authorization</span></span>  | <span data-ttu-id="e785d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e785d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e785d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e785d-124">Content-Type</span></span>   | <span data-ttu-id="e785d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e785d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e785d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e785d-127">Request body</span></span>

<span data-ttu-id="e785d-128">В теле запроса поставляем JSON-представление [объекта personWebsite.](../resources/personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="e785d-128">In the request body, supply a JSON representation of the [personWebsite](../resources/personwebsite.md) object.</span></span>

<span data-ttu-id="e785d-129">В следующей таблице показаны свойства, которые можно задать в новом [объекте personWebsite](../resources/personwebsite.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="e785d-129">The following table shows the properties that are possible to set within a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="e785d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e785d-130">Property</span></span>|<span data-ttu-id="e785d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e785d-131">Type</span></span>|<span data-ttu-id="e785d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e785d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e785d-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="e785d-133">allowedAudiences</span></span>|<span data-ttu-id="e785d-134">String</span><span class="sxs-lookup"><span data-stu-id="e785d-134">String</span></span>|<span data-ttu-id="e785d-135">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="e785d-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e785d-136">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e785d-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e785d-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e785d-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e785d-138">categories</span><span class="sxs-lookup"><span data-stu-id="e785d-138">categories</span></span>|<span data-ttu-id="e785d-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e785d-139">String collection</span></span>|<span data-ttu-id="e785d-140">Содержит категории, связанные с веб-сайтом (например, личные, рецепты).</span><span class="sxs-lookup"><span data-stu-id="e785d-140">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>|
|<span data-ttu-id="e785d-141">description</span><span class="sxs-lookup"><span data-stu-id="e785d-141">description</span></span>|<span data-ttu-id="e785d-142">String</span><span class="sxs-lookup"><span data-stu-id="e785d-142">String</span></span>|<span data-ttu-id="e785d-143">Содержит описание веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="e785d-143">Contains a description of the website.</span></span>|
|<span data-ttu-id="e785d-144">displayName</span><span class="sxs-lookup"><span data-stu-id="e785d-144">displayName</span></span>|<span data-ttu-id="e785d-145">String</span><span class="sxs-lookup"><span data-stu-id="e785d-145">String</span></span>|<span data-ttu-id="e785d-146">Содержит удобное имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="e785d-146">Contains a friendly name for the website.</span></span>|
|<span data-ttu-id="e785d-147">вывод</span><span class="sxs-lookup"><span data-stu-id="e785d-147">inference</span></span>|[<span data-ttu-id="e785d-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="e785d-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e785d-149">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="e785d-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e785d-150">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e785d-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e785d-151">source</span><span class="sxs-lookup"><span data-stu-id="e785d-151">source</span></span>|[<span data-ttu-id="e785d-152">personDataSource</span><span class="sxs-lookup"><span data-stu-id="e785d-152">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="e785d-153">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="e785d-153">Where the values originated if synced from another service.</span></span> <span data-ttu-id="e785d-154">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="e785d-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e785d-155">webUrl</span><span class="sxs-lookup"><span data-stu-id="e785d-155">webUrl</span></span>|<span data-ttu-id="e785d-156">String</span><span class="sxs-lookup"><span data-stu-id="e785d-156">String</span></span>|<span data-ttu-id="e785d-157">Содержит ссылку на сам веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="e785d-157">Contains a link to the website itself.</span></span>|

## <a name="response"></a><span data-ttu-id="e785d-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="e785d-158">Response</span></span>

<span data-ttu-id="e785d-159">В случае успеха этот метод возвращает код ответа и `201, Created` новый [объект personWebsite](../resources/personwebsite.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e785d-159">If successful, this method returns `201, Created` response code and a new [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e785d-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="e785d-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e785d-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="e785d-161">Request</span></span>

<span data-ttu-id="e785d-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e785d-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e785d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="e785d-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personwebsite_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/websites
Content-type: application/json

{
  "categories": [
    "football"
  ],
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```
# <a name="c"></a>[<span data-ttu-id="e785d-164">C#</span><span class="sxs-lookup"><span data-stu-id="e785d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personwebsite-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e785d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e785d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personwebsite-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e785d-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e785d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personwebsite-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e785d-167">Java</span><span class="sxs-lookup"><span data-stu-id="e785d-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personwebsite-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e785d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="e785d-168">Response</span></span>

<span data-ttu-id="e785d-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e785d-169">The following is an example of the response.</span></span>

> <span data-ttu-id="e785d-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e785d-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 201 Created
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
    "football"
  ],
  "description": null,
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```


