---
title: Создание премий
description: Создание нового объекта премий.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0ab51df665b9114bc590199319073efd90b5385e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034513"
---
# <a name="create-personaward"></a><span data-ttu-id="ac85a-103">Создание Персонавард</span><span class="sxs-lookup"><span data-stu-id="ac85a-103">Create personAward</span></span>

<span data-ttu-id="ac85a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac85a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac85a-105">Создание нового объекта [персонавард](../resources/personaward.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac85a-105">Create a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac85a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac85a-106">Permissions</span></span>

<span data-ttu-id="ac85a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac85a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac85a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac85a-109">Permission type</span></span>                        | <span data-ttu-id="ac85a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac85a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ac85a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac85a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac85a-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ac85a-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ac85a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac85a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac85a-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ac85a-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ac85a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac85a-115">Application</span></span>                            | <span data-ttu-id="ac85a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac85a-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="ac85a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac85a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/awards
POST /users/{id | userPrincipalName}/profile/awards
```

## <a name="request-headers"></a><span data-ttu-id="ac85a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac85a-118">Request headers</span></span>
|<span data-ttu-id="ac85a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ac85a-119">Name</span></span>|<span data-ttu-id="ac85a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ac85a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ac85a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac85a-121">Authorization</span></span>|<span data-ttu-id="ac85a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac85a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ac85a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac85a-124">Content-Type</span></span>|<span data-ttu-id="ac85a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac85a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac85a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac85a-127">Request body</span></span>
<span data-ttu-id="ac85a-128">В тексте запроса добавьте представление объекта [персонавард](../resources/personaward.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac85a-128">In the request body, supply a JSON representation of the [personAward](../resources/personaward.md) object.</span></span>

<span data-ttu-id="ac85a-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [персонавард](../resources/personaward.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac85a-129">The following table shows the properties that are possible to set when creating a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="ac85a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac85a-130">Property</span></span>|<span data-ttu-id="ac85a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ac85a-131">Type</span></span>|<span data-ttu-id="ac85a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ac85a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac85a-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="ac85a-133">allowedAudiences</span></span>|<span data-ttu-id="ac85a-134">String</span><span class="sxs-lookup"><span data-stu-id="ac85a-134">String</span></span>|<span data-ttu-id="ac85a-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="ac85a-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="ac85a-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ac85a-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="ac85a-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ac85a-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ac85a-138">description</span><span class="sxs-lookup"><span data-stu-id="ac85a-138">description</span></span>|<span data-ttu-id="ac85a-139">String</span><span class="sxs-lookup"><span data-stu-id="ac85a-139">String</span></span>|<span data-ttu-id="ac85a-140">Дескприптион вознаграждения или почетной грамоты.</span><span class="sxs-lookup"><span data-stu-id="ac85a-140">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="ac85a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="ac85a-141">displayName</span></span>|<span data-ttu-id="ac85a-142">String</span><span class="sxs-lookup"><span data-stu-id="ac85a-142">String</span></span>|<span data-ttu-id="ac85a-143">Название вознаграждения или соблюдается.</span><span class="sxs-lookup"><span data-stu-id="ac85a-143">Name of the award or honor.</span></span> |
|<span data-ttu-id="ac85a-144">выводов</span><span class="sxs-lookup"><span data-stu-id="ac85a-144">inference</span></span>|[<span data-ttu-id="ac85a-145">инференцедата</span><span class="sxs-lookup"><span data-stu-id="ac85a-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="ac85a-146">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="ac85a-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="ac85a-147">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ac85a-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ac85a-148">иссуеддате</span><span class="sxs-lookup"><span data-stu-id="ac85a-148">issuedDate</span></span>|<span data-ttu-id="ac85a-149">Дата</span><span class="sxs-lookup"><span data-stu-id="ac85a-149">Date</span></span>|<span data-ttu-id="ac85a-150">Дата предоставления вознаграждения или почетной грамоты.</span><span class="sxs-lookup"><span data-stu-id="ac85a-150">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="ac85a-151">иссуингаусорити</span><span class="sxs-lookup"><span data-stu-id="ac85a-151">issuingAuthority</span></span>|<span data-ttu-id="ac85a-152">String</span><span class="sxs-lookup"><span data-stu-id="ac85a-152">String</span></span>|<span data-ttu-id="ac85a-153">Орган, которому предоставлена премия или соблюдается.</span><span class="sxs-lookup"><span data-stu-id="ac85a-153">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="ac85a-154">source</span><span class="sxs-lookup"><span data-stu-id="ac85a-154">source</span></span>|[<span data-ttu-id="ac85a-155">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="ac85a-155">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="ac85a-156">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="ac85a-156">Where the values originated if synced from another service.</span></span> <span data-ttu-id="ac85a-157">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ac85a-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ac85a-158">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="ac85a-158">thumbnailUrl</span></span>|<span data-ttu-id="ac85a-159">String</span><span class="sxs-lookup"><span data-stu-id="ac85a-159">String</span></span>|<span data-ttu-id="ac85a-160">URL-адрес, ссылающийся на эскиз вознаграждения или соблюдается.</span><span class="sxs-lookup"><span data-stu-id="ac85a-160">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="ac85a-161">webUrl</span><span class="sxs-lookup"><span data-stu-id="ac85a-161">webUrl</span></span>|<span data-ttu-id="ac85a-162">String</span><span class="sxs-lookup"><span data-stu-id="ac85a-162">String</span></span>|<span data-ttu-id="ac85a-163">URL-адрес, ссылающийся на награду или соблюдать.</span><span class="sxs-lookup"><span data-stu-id="ac85a-163">URL referencing the award or honor.</span></span> |

## <a name="response"></a><span data-ttu-id="ac85a-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac85a-164">Response</span></span>

<span data-ttu-id="ac85a-165">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [персонавард](../resources/personaward.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac85a-165">If successful, this method returns a `201 Created` response code and an [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac85a-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="ac85a-166">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="ac85a-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac85a-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personaward_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/awards
Content-Type: application/json
Content-length: 497

{
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[<span data-ttu-id="ac85a-168">C#</span><span class="sxs-lookup"><span data-stu-id="ac85a-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personaward-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac85a-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac85a-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personaward-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac85a-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac85a-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personaward-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ac85a-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac85a-171">Response</span></span>
<span data-ttu-id="ac85a-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac85a-172">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
}
-->
``` http
HTTP/1.1 201 Created
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


