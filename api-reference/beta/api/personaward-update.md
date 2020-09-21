---
title: Обновление Персонавард
description: Обновление свойств объекта Персонавард.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1338c1990ad76611295ac34e13b30b53651839d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969321"
---
# <a name="update-personaward"></a><span data-ttu-id="993e5-103">Обновление Персонавард</span><span class="sxs-lookup"><span data-stu-id="993e5-103">Update personAward</span></span>

<span data-ttu-id="993e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="993e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="993e5-105">Обновление свойств объекта [персонавард](../resources/personAward.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="993e5-105">Update the properties of a [personAward](../resources/personAward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="993e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="993e5-106">Permissions</span></span>

<span data-ttu-id="993e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="993e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="993e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="993e5-109">Permission type</span></span>                        | <span data-ttu-id="993e5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="993e5-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="993e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="993e5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="993e5-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="993e5-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="993e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="993e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="993e5-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="993e5-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="993e5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="993e5-115">Application</span></span>                            | <span data-ttu-id="993e5-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="993e5-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="993e5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="993e5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/awards/{id}
PATCH /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="request-headers"></a><span data-ttu-id="993e5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="993e5-118">Request headers</span></span>
|<span data-ttu-id="993e5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="993e5-119">Name</span></span>|<span data-ttu-id="993e5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="993e5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="993e5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="993e5-121">Authorization</span></span>|<span data-ttu-id="993e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="993e5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="993e5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="993e5-124">Content-Type</span></span>|<span data-ttu-id="993e5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="993e5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="993e5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="993e5-127">Request body</span></span>

<span data-ttu-id="993e5-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="993e5-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="993e5-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="993e5-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="993e5-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="993e5-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="993e5-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="993e5-131">Property</span></span>|<span data-ttu-id="993e5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="993e5-132">Type</span></span>|<span data-ttu-id="993e5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="993e5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="993e5-134">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="993e5-134">allowedAudiences</span></span>|<span data-ttu-id="993e5-135">String</span><span class="sxs-lookup"><span data-stu-id="993e5-135">String</span></span>|<span data-ttu-id="993e5-136">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="993e5-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="993e5-137">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="993e5-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="993e5-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="993e5-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="993e5-139">description</span><span class="sxs-lookup"><span data-stu-id="993e5-139">description</span></span>|<span data-ttu-id="993e5-140">String</span><span class="sxs-lookup"><span data-stu-id="993e5-140">String</span></span>|<span data-ttu-id="993e5-141">Дескприптион вознаграждения или почетной грамоты.</span><span class="sxs-lookup"><span data-stu-id="993e5-141">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="993e5-142">displayName</span><span class="sxs-lookup"><span data-stu-id="993e5-142">displayName</span></span>|<span data-ttu-id="993e5-143">String</span><span class="sxs-lookup"><span data-stu-id="993e5-143">String</span></span>|<span data-ttu-id="993e5-144">Название вознаграждения или соблюдается.</span><span class="sxs-lookup"><span data-stu-id="993e5-144">Name of the award or honor.</span></span> |
|<span data-ttu-id="993e5-145">выводов</span><span class="sxs-lookup"><span data-stu-id="993e5-145">inference</span></span>|[<span data-ttu-id="993e5-146">инференцедата</span><span class="sxs-lookup"><span data-stu-id="993e5-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="993e5-147">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="993e5-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="993e5-148">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="993e5-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="993e5-149">иссуеддате</span><span class="sxs-lookup"><span data-stu-id="993e5-149">issuedDate</span></span>|<span data-ttu-id="993e5-150">Дата</span><span class="sxs-lookup"><span data-stu-id="993e5-150">Date</span></span>|<span data-ttu-id="993e5-151">Дата предоставления вознаграждения или почетной грамоты.</span><span class="sxs-lookup"><span data-stu-id="993e5-151">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="993e5-152">иссуингаусорити</span><span class="sxs-lookup"><span data-stu-id="993e5-152">issuingAuthority</span></span>|<span data-ttu-id="993e5-153">String</span><span class="sxs-lookup"><span data-stu-id="993e5-153">String</span></span>|<span data-ttu-id="993e5-154">Орган, которому предоставлена премия или соблюдается.</span><span class="sxs-lookup"><span data-stu-id="993e5-154">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="993e5-155">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="993e5-155">thumbnailUrl</span></span>|<span data-ttu-id="993e5-156">String</span><span class="sxs-lookup"><span data-stu-id="993e5-156">String</span></span>|<span data-ttu-id="993e5-157">URL-адрес, ссылающийся на эскиз вознаграждения или соблюдается.</span><span class="sxs-lookup"><span data-stu-id="993e5-157">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="993e5-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="993e5-158">webUrl</span></span>|<span data-ttu-id="993e5-159">String</span><span class="sxs-lookup"><span data-stu-id="993e5-159">String</span></span>|<span data-ttu-id="993e5-160">URL-адрес, ссылающийся на награду или соблюдать.</span><span class="sxs-lookup"><span data-stu-id="993e5-160">URL referencing the award or honor.</span></span> |

## <a name="response"></a><span data-ttu-id="993e5-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="993e5-161">Response</span></span>

<span data-ttu-id="993e5-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонавард](../resources/personaward.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="993e5-162">If successful, this method returns a `200 OK` response code and an updated [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="993e5-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="993e5-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="993e5-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="993e5-164">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="993e5-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="993e5-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personaward"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/awards/{personAwardId}
Content-Type: application/json
Content-length: 497

{
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg"
}
```
# <a name="c"></a>[<span data-ttu-id="993e5-166">C#</span><span class="sxs-lookup"><span data-stu-id="993e5-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="993e5-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="993e5-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="993e5-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="993e5-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="993e5-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="993e5-169">Response</span></span>
<span data-ttu-id="993e5-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="993e5-170">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```


