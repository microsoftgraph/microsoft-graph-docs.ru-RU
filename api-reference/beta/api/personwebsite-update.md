---
title: Обновление Персонвебсите
description: Обновление свойств объекта Персонвебсите в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 33b99ded6830a3e9ed4cd985be760824f18e8ee6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010656"
---
# <a name="update-personwebsite"></a><span data-ttu-id="8cdfb-103">Обновление персонвебсите</span><span class="sxs-lookup"><span data-stu-id="8cdfb-103">Update personwebsite</span></span>

<span data-ttu-id="8cdfb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cdfb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cdfb-105">Обновление свойств объекта [персонвебсите](../resources/personwebsite.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-105">Update the properties of [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8cdfb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cdfb-106">Permissions</span></span>

<span data-ttu-id="8cdfb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cdfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8cdfb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cdfb-109">Permission type</span></span>                        | <span data-ttu-id="8cdfb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cdfb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8cdfb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cdfb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cdfb-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8cdfb-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8cdfb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cdfb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cdfb-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8cdfb-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8cdfb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cdfb-115">Application</span></span>                            | <span data-ttu-id="8cdfb-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cdfb-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8cdfb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cdfb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/websites/{id}
PATCH /users/{id | userPrincipalName}/profile/websites/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8cdfb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cdfb-118">Request headers</span></span>

| <span data-ttu-id="8cdfb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8cdfb-119">Name</span></span>           |<span data-ttu-id="8cdfb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8cdfb-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="8cdfb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8cdfb-121">Authorization</span></span>  | <span data-ttu-id="8cdfb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8cdfb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cdfb-124">Content-Type</span></span>   | <span data-ttu-id="8cdfb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cdfb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cdfb-127">Request body</span></span>

<span data-ttu-id="8cdfb-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8cdfb-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8cdfb-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="8cdfb-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cdfb-131">Property</span></span>|<span data-ttu-id="8cdfb-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8cdfb-132">Type</span></span>|<span data-ttu-id="8cdfb-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8cdfb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cdfb-134">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="8cdfb-134">allowedAudiences</span></span>|<span data-ttu-id="8cdfb-135">String</span><span class="sxs-lookup"><span data-stu-id="8cdfb-135">String</span></span>|<span data-ttu-id="8cdfb-136">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8cdfb-137">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8cdfb-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8cdfb-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8cdfb-139">categories</span><span class="sxs-lookup"><span data-stu-id="8cdfb-139">categories</span></span>|<span data-ttu-id="8cdfb-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8cdfb-140">String collection</span></span>|<span data-ttu-id="8cdfb-141">Содержит категории, связанные с веб-сайтом пользователя (например, персональный, рецепты).</span><span class="sxs-lookup"><span data-stu-id="8cdfb-141">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>|
|<span data-ttu-id="8cdfb-142">description</span><span class="sxs-lookup"><span data-stu-id="8cdfb-142">description</span></span>|<span data-ttu-id="8cdfb-143">String</span><span class="sxs-lookup"><span data-stu-id="8cdfb-143">String</span></span>|<span data-ttu-id="8cdfb-144">Содержит описание веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-144">Contains a description of the website.</span></span>|
|<span data-ttu-id="8cdfb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8cdfb-145">displayName</span></span>|<span data-ttu-id="8cdfb-146">String</span><span class="sxs-lookup"><span data-stu-id="8cdfb-146">String</span></span>|<span data-ttu-id="8cdfb-147">Содержит понятное имя для веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-147">Contains a friendly name for the website.</span></span>|
|<span data-ttu-id="8cdfb-148">выводов</span><span class="sxs-lookup"><span data-stu-id="8cdfb-148">inference</span></span>|[<span data-ttu-id="8cdfb-149">инференцедата</span><span class="sxs-lookup"><span data-stu-id="8cdfb-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8cdfb-150">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8cdfb-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8cdfb-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8cdfb-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="8cdfb-152">webUrl</span></span>|<span data-ttu-id="8cdfb-153">String</span><span class="sxs-lookup"><span data-stu-id="8cdfb-153">String</span></span>|<span data-ttu-id="8cdfb-154">Содержит ссылку на сам веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-154">Contains a link to the website itself.</span></span>|

## <a name="response"></a><span data-ttu-id="8cdfb-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cdfb-155">Response</span></span>

<span data-ttu-id="8cdfb-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонвебсите](../resources/personwebsite.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-156">If successful, this method returns a `200 OK` response code and an updated [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8cdfb-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="8cdfb-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8cdfb-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cdfb-158">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="8cdfb-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cdfb-159">HTTP</span></span>](#tab/http)

<span data-ttu-id="8cdfb-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-160">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_personwebsite"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/websites/{id}
Content-type: application/json

{
  "description": "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
}
```
# <a name="c"></a>[<span data-ttu-id="8cdfb-161">C#</span><span class="sxs-lookup"><span data-stu-id="8cdfb-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personwebsite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cdfb-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cdfb-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personwebsite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cdfb-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cdfb-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personwebsite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8cdfb-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cdfb-164">Response</span></span>

<span data-ttu-id="8cdfb-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-165">The following is an example of the response.</span></span>

> <span data-ttu-id="8cdfb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8cdfb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
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
    "football"
  ],
  "description": "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway",
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```


