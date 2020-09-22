---
title: Обновление Персонинтерест
description: Обновление свойств объекта Персонинтерест.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 812a692a721e9d9a76cb7a0fa2547e48fb849e1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067939"
---
# <a name="update-personinterest"></a><span data-ttu-id="ad568-103">Обновление персонинтерест</span><span class="sxs-lookup"><span data-stu-id="ad568-103">Update personinterest</span></span>

<span data-ttu-id="ad568-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad568-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad568-105">Обновление свойств объекта [персонинтерест](../resources/personinterest.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ad568-105">Update the properties of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad568-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad568-106">Permissions</span></span>

<span data-ttu-id="ad568-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad568-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad568-109">Permission type</span></span>                        | <span data-ttu-id="ad568-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad568-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ad568-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad568-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad568-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ad568-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ad568-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad568-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad568-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ad568-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ad568-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad568-115">Application</span></span>                            | <span data-ttu-id="ad568-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad568-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="ad568-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad568-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/interests/{id}
PATCH /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ad568-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad568-118">Request headers</span></span>

| <span data-ttu-id="ad568-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ad568-119">Name</span></span>           |<span data-ttu-id="ad568-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ad568-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ad568-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad568-121">Authorization</span></span>  | <span data-ttu-id="ad568-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad568-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ad568-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad568-124">Content-Type</span></span>   | <span data-ttu-id="ad568-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad568-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad568-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad568-127">Request body</span></span>

<span data-ttu-id="ad568-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ad568-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ad568-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="ad568-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ad568-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ad568-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="ad568-131">В следующей таблице приведены свойства, которые можно обновлять в существующем объекте [персонинтерест](../resources/personinterest.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ad568-131">The following table shows the properties that are possible to update within an existing [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="ad568-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad568-132">Property</span></span>|<span data-ttu-id="ad568-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ad568-133">Type</span></span>|<span data-ttu-id="ad568-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ad568-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad568-135">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="ad568-135">allowedAudiences</span></span>|<span data-ttu-id="ad568-136">String</span><span class="sxs-lookup"><span data-stu-id="ad568-136">String</span></span>|<span data-ttu-id="ad568-137">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="ad568-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="ad568-138">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ad568-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="ad568-139">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ad568-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ad568-140">categories</span><span class="sxs-lookup"><span data-stu-id="ad568-140">categories</span></span>|<span data-ttu-id="ad568-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ad568-141">String collection</span></span>|<span data-ttu-id="ad568-142">Содержит категории, которые пользователь связал с интересом (например, персональный, реЦипиес).</span><span class="sxs-lookup"><span data-stu-id="ad568-142">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="ad568-143">коллаборатионтагс</span><span class="sxs-lookup"><span data-stu-id="ad568-143">collaborationTags</span></span>|<span data-ttu-id="ad568-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ad568-144">String collection</span></span>|<span data-ttu-id="ad568-145">Содержит теги сценариев, с которыми пользователь связан с интересом.</span><span class="sxs-lookup"><span data-stu-id="ad568-145">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="ad568-146">Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="ad568-146">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="ad568-147">description</span><span class="sxs-lookup"><span data-stu-id="ad568-147">description</span></span>|<span data-ttu-id="ad568-148">String</span><span class="sxs-lookup"><span data-stu-id="ad568-148">String</span></span>|<span data-ttu-id="ad568-149">Содержит описание интереса.</span><span class="sxs-lookup"><span data-stu-id="ad568-149">Contains a description of the interest.</span></span>|
|<span data-ttu-id="ad568-150">displayName</span><span class="sxs-lookup"><span data-stu-id="ad568-150">displayName</span></span>|<span data-ttu-id="ad568-151">String</span><span class="sxs-lookup"><span data-stu-id="ad568-151">String</span></span>|<span data-ttu-id="ad568-152">Содержит понятное имя для интереса.</span><span class="sxs-lookup"><span data-stu-id="ad568-152">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="ad568-153">выводов</span><span class="sxs-lookup"><span data-stu-id="ad568-153">inference</span></span>|[<span data-ttu-id="ad568-154">инференцедата</span><span class="sxs-lookup"><span data-stu-id="ad568-154">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="ad568-155">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="ad568-155">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="ad568-156">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ad568-156">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ad568-157">webUrl</span><span class="sxs-lookup"><span data-stu-id="ad568-157">webUrl</span></span>|<span data-ttu-id="ad568-158">String</span><span class="sxs-lookup"><span data-stu-id="ad568-158">String</span></span>|<span data-ttu-id="ad568-159">Содержит ссылку на веб-страницу или ресурс, представляющие интерес.</span><span class="sxs-lookup"><span data-stu-id="ad568-159">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="ad568-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad568-160">Response</span></span>

<span data-ttu-id="ad568-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонинтерест](../resources/personinterest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad568-161">If successful, this method returns a `200 OK` response code and an updated [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad568-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="ad568-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ad568-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad568-163">Request</span></span>

<span data-ttu-id="ad568-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad568-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad568-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad568-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ad568-166">C#</span><span class="sxs-lookup"><span data-stu-id="ad568-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad568-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad568-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad568-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad568-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad568-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad568-169">Response</span></span>

<span data-ttu-id="ad568-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad568-170">The following is an example of the response.</span></span>

> <span data-ttu-id="ad568-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad568-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


