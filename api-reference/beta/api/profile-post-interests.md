---
title: Создание personInterest
description: Создайте новый personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: e4f5648901ff1ed904d5e02fa278b6b9be329de8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036928"
---
# <a name="create-personinterest"></a><span data-ttu-id="5d946-103">Создание personInterest</span><span class="sxs-lookup"><span data-stu-id="5d946-103">Create personInterest</span></span>

<span data-ttu-id="5d946-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d946-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d946-105">Создание нового [personInterest].. /resources/personinterest.md] в профиле [пользователя](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="5d946-105">Create a new [personInterest](../resources/personinterest.md] in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d946-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d946-106">Permissions</span></span>

<span data-ttu-id="5d946-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d946-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d946-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d946-109">Permission type</span></span>                        | <span data-ttu-id="5d946-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d946-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d946-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d946-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d946-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d946-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5d946-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d946-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d946-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d946-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5d946-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d946-115">Application</span></span>                            | <span data-ttu-id="5d946-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d946-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="5d946-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d946-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/interests
POST /users/{id | userPrincipalName}/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="5d946-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d946-118">Request headers</span></span>

| <span data-ttu-id="5d946-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5d946-119">Name</span></span>      |<span data-ttu-id="5d946-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5d946-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d946-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d946-121">Authorization</span></span>  | <span data-ttu-id="5d946-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d946-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5d946-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d946-124">Content-Type</span></span>   | <span data-ttu-id="5d946-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d946-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d946-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d946-127">Request body</span></span>

<span data-ttu-id="5d946-128">В теле запроса поставляют представление JSON объекта [personInterest.](../resources/personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="5d946-128">In the request body, supply a JSON representation of the [personInterest](../resources/personinterest.md) object.</span></span>

<span data-ttu-id="5d946-129">В следующей таблице показаны свойства, которые можно установить в новом [объекте personInterest](../resources/personinterest.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="5d946-129">The following table shows the properties that are possible to set within a new [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="5d946-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d946-130">Property</span></span>|<span data-ttu-id="5d946-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5d946-131">Type</span></span>|<span data-ttu-id="5d946-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5d946-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d946-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="5d946-133">allowedAudiences</span></span>|<span data-ttu-id="5d946-134">String</span><span class="sxs-lookup"><span data-stu-id="5d946-134">String</span></span>|<span data-ttu-id="5d946-135">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="5d946-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="5d946-136">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5d946-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="5d946-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5d946-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5d946-138">categories</span><span class="sxs-lookup"><span data-stu-id="5d946-138">categories</span></span>|<span data-ttu-id="5d946-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5d946-139">String collection</span></span>|<span data-ttu-id="5d946-140">Содержит категории, связанные с интересом пользователя (например, личные, личные).</span><span class="sxs-lookup"><span data-stu-id="5d946-140">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="5d946-141">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="5d946-141">collaborationTags</span></span>|<span data-ttu-id="5d946-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5d946-142">String collection</span></span>|<span data-ttu-id="5d946-143">Содержит теги сценариев работы, которые пользователь связал с интересом.</span><span class="sxs-lookup"><span data-stu-id="5d946-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="5d946-144">Допустимые значения в коллекции: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="5d946-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="5d946-145">description</span><span class="sxs-lookup"><span data-stu-id="5d946-145">description</span></span>|<span data-ttu-id="5d946-146">String</span><span class="sxs-lookup"><span data-stu-id="5d946-146">String</span></span>|<span data-ttu-id="5d946-147">Содержит описание интерес.</span><span class="sxs-lookup"><span data-stu-id="5d946-147">Contains a description of the interest.</span></span>|
|<span data-ttu-id="5d946-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5d946-148">displayName</span></span>|<span data-ttu-id="5d946-149">String</span><span class="sxs-lookup"><span data-stu-id="5d946-149">String</span></span>|<span data-ttu-id="5d946-150">Содержит удобное имя для интереса.</span><span class="sxs-lookup"><span data-stu-id="5d946-150">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="5d946-151">вывод</span><span class="sxs-lookup"><span data-stu-id="5d946-151">inference</span></span>|[<span data-ttu-id="5d946-152">inferenceData</span><span class="sxs-lookup"><span data-stu-id="5d946-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="5d946-153">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="5d946-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="5d946-154">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5d946-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5d946-155">source</span><span class="sxs-lookup"><span data-stu-id="5d946-155">source</span></span>|[<span data-ttu-id="5d946-156">personDataSource</span><span class="sxs-lookup"><span data-stu-id="5d946-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="5d946-157">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="5d946-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="5d946-158">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5d946-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5d946-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="5d946-159">webUrl</span></span>|<span data-ttu-id="5d946-160">String</span><span class="sxs-lookup"><span data-stu-id="5d946-160">String</span></span>|<span data-ttu-id="5d946-161">Содержит ссылку на веб-страницу или ресурс об интересе.</span><span class="sxs-lookup"><span data-stu-id="5d946-161">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="5d946-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d946-162">Response</span></span>

<span data-ttu-id="5d946-163">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект personInterest](../resources/personinterest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5d946-163">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d946-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="5d946-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d946-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d946-165">Request</span></span>

<span data-ttu-id="5d946-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d946-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d946-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d946-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personinterest_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/interests
Content-type: application/json

{
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com"
}
```
# <a name="c"></a>[<span data-ttu-id="5d946-168">C#</span><span class="sxs-lookup"><span data-stu-id="5d946-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d946-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d946-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d946-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d946-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d946-171">Java</span><span class="sxs-lookup"><span data-stu-id="5d946-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personinterest-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d946-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d946-172">Response</span></span>

<span data-ttu-id="5d946-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5d946-173">The following is an example of the response.</span></span>

> <span data-ttu-id="5d946-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5d946-174">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
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
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


